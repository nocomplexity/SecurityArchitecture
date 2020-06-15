Zero trust architecture design principles
----------------------------------------------

(The original input for this subsection is retrieved from https://github.com/ukncsc/zero-trust-architecture )

Rationale for the zero trust principles

The traditional network perimeter is disappearing and with it, the value of traditional defences.
In a zero trust architecture, inherent trust is removed from the network. Just because you're connected to a network doesn't mean you should be able to access everything on that network. This is commonly seen in breaches; an attacker gains a foothold in a network and is able to move laterally because everything on the network is trusted. In a zero trust architecture, the network is treated as hostile.

However, in order to remove trust from the network, you need to instead gain confidence in the authentication, verification and authorization of users and services. This is achieved by building trust into the user's identity (user authentication), their devices (device verification), and the services they access (service authorisation). For this model to be effective, each connection to a service should be authenticated and the device and connection authorised against a policy, regardless of where the connection request comes from. 

To enable authorisation decisions, access policies need to be defined, based on who can access which service or data, under which circumstances. How much confidence you need to trust a connection depends on the value of data being accessed or impact of action being performed. Likewise, devices should be inventoried and device verification should be based on defined policies (such as encryption, patch levels, etc).

These principles, like all security principles, are intended to help you design and deploy a secure end-to-end, zero trust architecture. 

Many of the zero trust principles outlined below can’t be fully satisfied with current, commercially available offerings. As always in security architecture, a risk managed approach is required.

Know your architecture including users, devices, and services
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In the zero trust network model it’s more important than ever to know about your assets. In order to get the benefits from zero trust you need to know about each component of your architecture from users and their devices, through to the services and data they are accessing.

Your attention should be focused on the components of the system which use the network. The network itself should be considered untrusted and hostile, regardless of whether it’s a local networking in your secure building, or a public Wi-Fi network in a known hostile location.

This principle is particularly important if transitioning to a zero trust architecture for an established system, with many pre-existing services. If a zero trust architecture is implemented without considering existing services, they may be at higher risk as the network is assumed to be untrusted and hostile. These services may not be designed for this situation and therefore will be unable to defend themselves against attack.

Create a single strong user identity
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Your organisation should use a single user directory and create accounts that are linked to individuals.

To enable granular access control, create specific roles for each user. Ensure the directory can be employed by all the services you plan to use, both internal and external. This will also help when accessing other organisation's services and data.

**Desirable features of an identity service include:**

* Create groups
* Define roles
* Support for strong, modern authentication methods such as multi-factor authentication or even passwordless authentication
* Easily, but securely, distribute credentials to users
* Authenticate to external services (e.g. SAML 2.0 or OpenID Connect)
* Manage user identities in external services (e.g. SCIM 2.0)
* Support for your joiners, movers, and leavers processes

If you have an existing directory, migrating to another directory will require careful planning. Some directory services allow you to import, synchronise or federate between directories, this would allow a phased approach to migration from your legacy directory service to one which supports a zero trust architecture.

Service accounts, keys, tokens and so on, should also be created in a central directory, with tightly defined permissions which are the minimum necessary to allow the service to function properly.

You should also consider how you’ll offer access to the resources your organisation controls, to people from outside your organisation. Your services should be able to use external identity providers to allow access to appropriate services and data. For example, a visitor can see the lunch menu, or a contractor can only access documents related to their work.

Identity is a wide-ranging topic and needs careful consideration as it's a foundational service for zero trust architectures. The NCSC has more in-depth [guidance on identity and access management](https://www.ncsc.gov.uk/guidance/introduction-identity-and-access-management).

Don't impersonate users: Do not empower services to take actions on behalf of end-users without their consent. A strong user identity is undone when components of a network can impersonate your users.

In applications and systems with multiple components, it is common for an application to need to make a request on behalf of an end user to another service to fulfill this users request.

An application making a call on behalf of the end-user may have to authenticate itself to a back end service to make the request, but if there is no artifact of an end-user request associated with this request to the back end, then we have empowered this application or any adversary in control of it to impersonate end users within the architecture.

Wherever possible, artifacts of end-user consent should be included with requests to back end services so that we can have greater confidence that this request originated from the end-user. This is best displayed in the RFC standard for "OAuth Token Exchange", where a system must use the end-user's Access Token and authenticate itself to a central authorization server for the right to call a back end service on behalf of an end-user.


Please note it is not desireable to replay artifacts like an end-user's session token to the front-end application within a system as this increases the chance that it may become compromised.


Create a strong device identity
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Each device owned by your organisation should be uniquely identifiable in a single device directory. This enables efficient asset management and clear visibility of the devices which access services and your data.

Policies you define later will use compliance and health claims from a device to make decisions about which data it can access and the actions it can perform. A strong identity is required to ensure these claims can be authenticated.

The confidence you can have in a device’s identity depends on the device type, hardware and platform:

* Identity stored on a secure hardware co-processor, like a TPM, will give you high confidence in the device’s identity
* Identity stored on a well-managed device using a software-based key store gives a lower confidence in the device’s identity
* Identity on an unmanaged device in a software-based key store gives a low confidence in the device’s identity

When allowing requests from devices you don’t own and manage, identification can be challenging. Devices in a BYOD model should still have an identity linked to them but the confidence in that device’s identity may be lower.

Identifying devices from another organisation will require a trust relationship to be established between the two organisations. This should happen at both a governance and technical level.

Authenticate everywhere
^^^^^^^^^^^^^^^^^^^^^^^^

In a zero trust architecture, assume the network is hostile and authenticate all connections.

Services may be available directly over the internet, so authentication of user requests requires a stronger mechanism than a simple username and password combination.

Multi-factor authentication is a requirement for a zero trust architecture. This doesn’t mean that the user experience has to be poor. On modern devices and platforms, strong multi-factor authentication can be achieved with a good user experience.

Consider adding additional factors depending on the impact of the request,like using tokens or one-time passwords, device type and state, physical location and user behaviour analytics.

It’s important that strong authentication doesn’t hinder the usability of a service. So, only prompt for additional authentication factors when requests are of high impact or importance. For example, when accessing sensitive data or requesting privileged actions, such as creating users.

Passwordless authentication (e.g. FIDO2) is an ideal solution which provides strong security with an excellent user experience. Consider implementing passwordless authentication for a strong, consistent, and simple authentication experience across all of your services.

Requests between services also need to be authenticated. This is normally achieved using API tokens, frameworks such as OAuth or Public Key Infrastructure (PKI). Use mutual authentication wherever possible.

Know the health of your devices and services
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The health of devices and services is one of the most important signals used to gain confidence in them.
Devices

Determining if the device accessing your services is up-to-date, compliant with your device configuration policies and in a healthy state is important as these represent some of the most important signals used to control access to services and data.

First, define policies which configure devices to be secure, NCSC’s end-user device guidance can help. Using a device management service, apply these policies to devices and enforce them, then continuously check that devices are compliant.

Device health consists of compliance with device configuration and device state. Is the device compliant with the policies that you set? Is the device in the expected state?

Device state can be determined based on the state of security features on the platform. For example, is secure boot enabled? Are the latest operating system updates installed? Is virtualisation-based security or system integrity protection enabled?

Going further, determining the underlaying state of a devices’ firmware, BIOS, and operating system kernel are strong signals which contributes to determining its overall health. Attestation is a way of achieving this, taking a snapshot of the state of a device with claims about different components of the hardware and operating system, that are reported to the signal database for analysis.

Systems that implement attestation to gain confidence in initial device state, may include subsequent cryptographic checks of launched applications and services to extend the breadth of health measurements regarded as strong signals.
Services

The health of services should also be considered, not only when end-user devices are accessing services but also when services are talking to other services. The supporting zero trust infrastructure, such as the policy engine and policy enforcement points should also be considered services when reading this principle.

Services should be configured to use their native security functions as per documentation and to satisfy the principles of zero trust. For instance, enforcing strong authentication mechanisms and disabling legacy protocol that don't support modern authentication.

Services also need to be kept up-to-date with the latest software patches and you need to be able to determine the version and patch level of the service you are using. Patches fixing vulnerabilities should applied at the earliest opportunity.

The health of your services needs to be monitored, an unexpected change in state may indicate an unauthorised change or malicious activity. How this is achieved will depend on the type of service, ideally this would be carried out programmatically by interrogating an API that the service provides.

Focus your monitoring on devices and services
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Given that devices and services are more exposed to network attacks than in traditional architectures, it’s important that comprehensive monitoring is carried out.

Focus on device and service monitoring; what are devices requesting from services, what actions are they performing, what data are they accessing. Your monitoring should link back to the policies that you set, verifying they are being enforced as you expect.

User devices within a traditional walled garden network architecture use a VPN to send all traffic through a controlled path, which enables traffic to be inspected. In a zero trust architecture, this chokepoint isn’t available and protective monitoring has to be moved onto each device.

Although the network is untrusted and assumed hostile, network monitoring is still important to ensure good performance and good cyber hygiene. Network monitoring should be carried out on your local networks to identify rogue devices and help identify malicious activity, especially if you’re hosting on-premise services. Coupled with device monitoring, network monitoring can help improve visibility and correlation; for example, you could trace network connections to the process on the device that generated them.

Set policies according to the value of services or data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The power of a zero trust architecture comes from the access policies you define. These policies can take into account a number of signals from the connection in real-time and from the signals database to a build context for the connection. This context is then used to gain confidence in the connection request and decide if it's trusted enough to continue. It's the role of the Policy Engine perform this policy decision.

In the previous principles we talked about building trust in a user’s identity, their devices and services. Signals from these sources can be used to make access decisions. For example, has a user authenticated using a second factor? Is the device they are using compliant with our configuration policies?

Define your policies based on the value of the data to be accessed or action taken. For example, a high impact action, such as creating a new administrator user, should require a stringent policy compared to a relatively low impact operation such as checking the lunch menu. In the latter example, the confidence required to trust the connection is relatively low.

Signals can include the user’s role, physical location, device state, value of the service they are accessing and risk of the action they are preforming. The richness of the policies you define is determined by the policy engine you are using and is closely linked to the user and device state signals available. When choosing which technologies to use for your zero trust architecture, evaluate the signals that are available and capabilities of your policy engine.

Depending on your policy engine's capabilities, you may be able to request additional signals in order to get more confidence in a connection. For example, if a user usually requests access to a high value service for the first time or outside of normal working hours your policy engine could ask for an additional factor of authentication.

Control access to your services and data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Each request to a service should be authorised against a policy. Use products and protocols that support this continuous authentication and authorisation process, while protecting your data in transit with encryption.

A zero trust architecture includes a component which mediates connections to services. This is a Policy Enforcement Point which actively applies the access policy you have defined based on a response from the Policy Engine.

How this is achieved practically depends on the zero trust supporting infrastructure you use and the flavour of zero trust technologies you deploy.

If using software defined perimeter (SDP), the policy enforcement point is usually the SDP controller that controls connections from a central location which may also be the Policy Engine. Enforcement points will focus on properties of the network connection to control access, for example which network protocols can be used, the origin of the connection, the network segments that can communicate based on the policy.

When using micro-segementation there is often a gateway in the form of a reverse proxy component. This component can enforce policy at many layers, from the network layer through to the application layer. At the application layer the gateway would need to understand the protocols being used by the application and how they are used. This may require complex logic in both the policy engine and the enforcement point.

Often in a cloud environment you may control access using an authentication and authorisation broker which provides single sign-on functionality to variety of applications. Enforcement is usually session based, policies will be assessed as a connection is established and the broker provides a short lived access token which allows users connect to the services they originally requested.

You may use a combination of the options above, or even different ways, to control access to your services and data. Regardless of how you design your zero trust architecture the component should only allow connections if the access policies you define are satisfied. As monitoring is important in a zero trust architecture your enforcement point should support logging connections and their properties.

Don’t trust the network, including the local network
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


In order to remove trust from the network you need to build trust into the devices and services.

Don’t trust any network between the device and the service it’s accessing. This includes the local network, the device should be configured to prevent DNS spoofing, Man in the Middle attacks, unsolicited inbound connections etc.

Attacks targeted at foundation network services, such as DNS, can often only be mitigated at higher layers in the stack, for example ensure that services your users are accessing are protected with authenticated and encrypted protocols, such as TLS.

While the network should be treated as hostile and untrusted, maintaining cyber hygiene and good standards on the network is still important ensuring they are performant and available. This is especially important in architectures where you are hosting on-premise services.

Choose services designed for zero trust
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Prefer services with built-in support for zero trust.

Some services, especially legacy services, may need additional components to enable zero trust. This may increase management overhead and cause usability issues, so ensure you have the resource to take this on.

Creating your own supporting infrastructure should be avoided, due to the cost, complexity and potential for error involved. In this case, as elsewhere, the general cyber security principle of “don’t roll your own” holds true.

Given that in a zero trust architecture, you can’t trust the network, services need to be designed to protect themselves from hostile networks. This includes the internet, to which components could be directly exposed.

Whenever possible, use standards-based technologies. This allows interoperability between devices and services. A good example is authentication, where common standards such as OpenID Connect or SAML allow you to use a single directory service to authenticate to many services.

Unfortunately, there are currently no standards for policies. We recommend that you use a single policy engine and apply the full set of features it offers.