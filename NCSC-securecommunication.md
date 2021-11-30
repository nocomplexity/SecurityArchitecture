# NCSC:Secure communication principles


Modern technology provides a wealth of options for communicating in the workplace, which now includes voice, email, group messaging, and video.

This guidance contains a set of principles that can help all organisations make sound security decisions when selecting the products and services that provide secure communications. It is aimed at risk owners and security professionals who wish to assess communication technologies for their organisations, to help them achieve the right balance of **functionality**, **security** and **privacy**.

It is of particular relevance for those working in government and the public sector.

*[source on github](https://github.com/ukncsc/secure-communication-principles/blob/master/README.md)*


## The NCSC's secure communication principles

1. Protect data in transit

2. Protect network nodes with access to sensitive data

3. Protect user access to the service 

4. Ensure secure audit of communications is provided

5. Allow administrators to securely manage users and systems

6. Use metadata only for its necessary purpose

7. Assess supply chain for trust and resilience

## 1. Protect data in transit

Is content protected against tampering and eavesdropping?

Communications will typically transit an untrusted network, such as the internet. An untrusted network is outside of your control, which means someone may be able to access (or modify) data transiting that network.

You can protect against tampering and eavesdropping by using a service that encrypts data as it travels between participants.

Can participants confirm who they are communicating with?

Communications can inadvertently be sent to the wrong recipient. This could be as simple as mistyping the recipient's details, which on some open services could result in sending information outside your organisation. Alternatively, recipients can 'spoof' other identities (i.e. pretend to be somebody they are not) and trick users into communicating with them. As a trusted recipient, it's then simple to share links to malicious websites, or spread misinformation.

You should use a service that offers authentication of other users, which allows a recipient to confirm a sender's identity.

## 2. Protect network nodes with access to sensitive data

Are network nodes with access to un-encrypted data protected appropriately?

Communications will typically transit a network, and in doing so they will pass through various servers and routers. Any of these network nodes with access to un-encrypted data may be able to access **all** communications between **all** users.

Network nodes that have access to un-encrypted data should be appropriately protected, at a level considerate of the impact of any compromise of communications. If the appropriate level of protection required for network nodes cannot be met, you should consider using a service that does not require un-encrypted communications data to pass through network nodes.

Are network nodes that manage cryptographic key material protected appropriately?

Communications normally rely on cryptography for security, with trust in the security relying on cryptographic keys. If someone gained access to the key management functionality in a service, then they could abuse this trust (for example to spoof any user, or potentially access their communications data).

As cryptographic key material often acts as the root of trust in a secure communications service, any part of the service involved in key management should be appropriately protected at a level considerate of the impact of compromise.

## 3. Protect user access to the service

Is user access to the service protected?

When a user sends content to another user, they will assume that only the true owner of the user's account will be able to access it. If someone else gains access to a user's account, they can impersonate them, see their communications, and send misinformation to other users.

User access to the service should be authenticated to ensure that only the intended users can access communications.

Is the user's device appropriately protected?

The device used to access a communications service will process un-encrypted data and may store user account credentials and historic communications content. If someone were able to gain a privileged status on the device, then they may be able to access the application (or its data store), which could allow them to impersonate the user (or access communications content).

Devices should be [appropriately configured](https://www.ncsc.gov.uk/collection/end-user-device-security) to protect against unauthorised access to the user account, and ensure that communications are kept private.

## 4. Ensure secure audit of communications is provided

Does the service provide access to communications content for audit purposes?

Communications services have scope to be misused, for example by spreading malware, or launching phishing attacks. Alternatively, insiders could leak privileged information, or commit financial fraud.

The communications service should provide audit functionality, so that organisations can provide improved security monitoring and also fulfil regulatory/legal requirements (such as investigating fraud or unlawful activities).

Is access to the audit functionality and communications content restricted?

Misuse of a service's audit functionality could allow unauthorised access to communications content. Only an authorised administrator, with appropriate permission and remit when access conditions are met, should be able to access communications content and associated metadata. Access to the audit functionality should be logged with a record of the activity performed, and the corresponding justification. The audit functionality provides access to sensitive data and so should meet principle 2 (protect network nodes with access to sensitive data).

## 5. Allow administrators to securely manage users and systems

Can administrators suitably manage their users' accounts?

If users are allowed to manage their own accounts, then an organisation will **not** have full control over how those accounts are accessed. Many organisations will need to manage how this is done, which could be as simple as a 'joiners and leavers' policy to ensure that users' accounts are revoked when they leave the organisation. Another example may be managing user access to different groups within the service, or granting permission to certain users so that they can set up groups.

The communications service should allow administrators to securely manage their organisation's users. Administrators should be able to manage user accounts throughout their lifecycle, giving them the required control to authorise or deny certain actions.

Is administration and management protected and restricted?

Access to the administration interface of the communications service could allow new accounts to be created and user access permissions to be changed. If someone gained control of this, they could create unauthorised accounts on the system, which could then be used nefariously. They could also disable legitimate accounts, or elevate the permission levels of users to subvert security controls.

Administration and management of the system should be restricted to authorised individuals, whose privileged access should be authenticated, using two-factor authentication if supported, and logged. In addition, the enrolment of users onto the service should require identification of the user to ensure they are authorised, before provisioning security credentials for the user account. Administration should also be practical for the scale of the organisation, to ensure that administrators do not take shortcuts in performing authorisation checks before carrying out administrator functions.

## 6. Use metadata only for its necessary purpose

Is the use of metadata well-understood and used only as is necessary?

When a communication is sent, the communications service needs certain metadata in order to operate. This includes user identifiers and timings (in other words, the 'who', 'where', 'when' and 'how' of the communication). This imparts information about users of the system, especially in aggregate, and if misused it could reveal the individual connections of users of the system.

You should ensure that such metadata is only used for the necessary operation of the service. In particular, that it is not harvested, sold or exploited by the communications service. The communications service should provide clear and transparent terms and conditions that set out what content and what metadata is collected and processed, and for what purpose. Moreover, you should have confidence that these will be followed and are appropriate for your corporate need, as opposed to a consumer need.

## 7. Assess supply chain for trust and resilience

Do you trust all components of the service?

If you do not have confidence in the security and operation of a component of the service, then any assessment of the service could be undermined. You should build trust with the service provider to ensure that you are content with their [supply chain security](https://www.ncsc.gov.uk/collection/supply-chain-security), including that of any third party products and services they rely on.

Can the actions of a single vendor impact security?

Communications services that are only supported by a single vendor carry certain risks with them. For example, there is a risk to the availability of the service if that vendor were to suffer a temporary outage, or go out of business entirely. Alternatively, the service may change and no longer meet these principles, if (for example) the vendor is taken over by another company.

You may prefer to use a standards-based communications service, which is supported by multiple vendors in an interoperable way. The existence of alternative providers reduces the dependence on a single vendor.

Are users able to communicate with contacts using different services?

Many organisations will wish to communicate securely with contacts outside of their own organisation. If a communications service does not allow this, then their members may revert to using an insecure service that does not meet these principles.

Where an organisation has requirements to securely communicate with people external to their organisation, they should choose a service that is interoperable with secure services used by partners.

