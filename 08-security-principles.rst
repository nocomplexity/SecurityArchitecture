Security Principles
===========================

**Address Privacy & Security** 
-----------------------------------

**Statement:** Address Privacy & Security

**Rationale:** Information is power and this is certainly true in the context of technology-enabled global development interventions. How information is collected, stored, analysed, shared, and used has serious implications for both the populations about whom data are being transmitted, and the organizations transmitting the data.

**Implications:** Assess and mitigate risks to the security of users and their data. Consider the context and needs for privacy of personally identifiable information when designing solutions and mitigate accordingly. Ensure equity and fairness in co-creation, and protect the best interests of the end end-users.




**Always consider the users** 
-------------------------------

**Statement:** Always consider the users

**Rationale:** The security of a software system is linked to what its users do with it. It is therefore important that all security-related mechanisms are designed in a manner that makes it easy for users to deploy, configure, use, and update the system securely. Security is not a feature that can simply be added to a software  system, but rather a property emerging from how the system was built and is operated. The way each user interacts with software is dictated not only by the design and implementation decisions of its creators but also by the cognitive abilities and cultural background of its users.

**Implications:** Failing to address this design principle can lead to a various problems, e.g.: When designers don’t “remember the user” in their software design, inadvertent disclosures by the user may take  place. If it is difficult to understand the authorization model, or difficult to understand the configuration for visibility  of data, then the user’s data are likely to be unintentionally disclosed. Designers sometimes fail to account for the fact that authenticated and properly authorized users can also be attackers! This design error is a failure to distrust the user, resulting in authorized users having opportunities to misuse the system. When security is too hard to set up for a large population of the system’s users, it will never be configured, or it will not be configured properly.




**Asset protection and resilience** 
-------------------------------------

**Statement:** Asset protection and resilience

**Rationale:** Consumer data, and the assets storing or processing it, should be protected against physical tampering, loss, damage or seizure.

**Implications:** If this principle is not implemented, inappropriately  data (e.g. user or consumer)  could be compromised which may result in legal and regulatory sanction, or reputation damage.




**Assume that external systems are insecure** 
-----------------------------------------------

**Statement:** Assume that external systems are insecure.

**Rationale:** The term information domain arises from the practice of partitioning information resources according to access control, need, and levels of protection required. Organizations implement specific measures to enforce this partitioning and to provide for the flow of authorized information between information domains. The boundary of an information domain represents the security perimeter for that domain. An external domain is one that is not under your control. In general, all external systems should be considered insecure.

**Implications:** Take proactive security measurements to protect secure data crossing information boundaries. Design secure information exchange interfaces (api's). Make agreements with parties involved. &nbsp;




**Audit information provision to consumers** 
----------------------------------------------

**Statement:** Audit information provision to consumers

**Rationale:** Consumers should be provided with the audit records they need to monitor access to their service and the data held within it. If this principle is not implemented, consumers will not be able to detect and respond to inappropriate or malicious use of their service or data within reasonable time-scales. In most countries this is a legal requirement from privacy point of view.

**Implications:** Secure audit mechanism needed. Requirements needed for audit data retention, storing, archiving.




**Authenticate users and processes** 
--------------------------------------

**Statement:** Authenticate users and processes to ensure appropriate access control decisions both within and across domains.

**Rationale:** Authentication is the process where a system establishes the validity of a transmission, message, or a means of verifying the eligibility of an individual, process, or machine to carry out a desired action, thereby ensuring that security is not compromised by an untrusted source. It is essential that adequate authentication be achieved in order to implement security policies and achieve security goals.

**Implications:** Authentication service needed for users and application processes. &nbsp;




**Authorize after you authenticate** 
--------------------------------------

**Statement:** Authorize after you authenticate.

**Rationale:** Authorization should be conducted as an explicit check, and as necessary even after an initial authentication has been completed. Authorization depends not only on the privileges associated with an authenticated user, but also on the context of the request. The time of the request and the location of the requesting user may both need to be taken into account.

**Implications:** For particularly sensitive operations, authorization may need to invoke authentication (again). Although authorization begins only after authentication has occurred, this requirement is not circular. Authentication is not binary—users may be required to present minimal (such as a password) or more substantial (e.g. biometric or token-based) evidence of their identity, and authentication in most systems is not continuous—a user may authenticate, but walk away from the device or hand it to someone else.




**Avoid security by obscurity** 
---------------------------------

**Statement:** Security measurements should be open and transparent.

**Rationale:** Assume attackers will have source code (also for closed source software). Assume attackers will have complete design and network topologies. Open security design promote cycle of improvement faster. Assume sensitive information regarding security measurements are leaked or sold.

**Implications:** Do not document secrets and configuration policies (settings) in security designs. Never store secrets (e.g. passwords) on systems. Involve internal and external SME to evaluate the strength and weakness of a security design. (design review). Security should always be tested by experts (open or not). Periodically pentest the security implementation, use different companies instead of always the same.




**Check the return value of functions** 
-----------------------------------------

**Statement:** Check the return value of all non-void functions, and check the validity of all function parameters. The return value of non-void functions must be checked by each calling function, and the validity of parameters must be checked inside each function.

**Rationale:** This is possibly the most frequently violated principle.In the strictest interpretation, this rule means that even the return value of printf statements and file close statements must be checked. A case can be made, though, that if the response to an error would rightfully be no different than the response to success, there is no point in checking a return value. This is often the case with calls to printf and close. In cases like these, it can be acceptable to explicitly cast the function return value to (void) -- thereby indicating that the programmer explicitly and not accidentally decides to ignore a return value. The rule is then only violated if the cast is missing. In more dubious cases, a comment should be present to explain why a return value is irrelevant. In most cases, though, the return value of a function should not be ignored, especially if error return values must be propagated up the function call chain. Standard libraries famously violate this rule with potentially grave consequences. See, for instance, what happens if you accidentally execute strlen(0), or strcat(s1, s2, -1) with the standard C string library. For this reason, most coding guidelines for safety critical software also forbid the use of all ansi standard headers like string.h, stdlib.h, stdio.h etc. If the function are needed, they should be written separately, and made compliant with safety critical use. The enforcement of this principle make sure that exceptions are always explicitly justified (and justifiable), with mechanical checkers flagging violations.  Often, it will be easier to comply with the rule than to explain why non-compliance is acceptable.

**Implications:** Extra testing and programming effort:Function parameters should normal be verified for validity before being used. This rule especially applies to pointers: before dereferencing a pointer that is passed as a parameter the pointer must be checked for null. Consider automating security testing on software (static and dynamic tests)




**Clearly delineate the physical and logical security boundaries** 
--------------------------------------------------------------------

**Statement:** Clearly delineate the physical and logical security boundaries governed by associated security policies.

**Rationale:** Information technology exists in physical and logical locations, and boundaries exist between these locations. An understanding of what is to be protected from external factors can help ensure adequate protective measures are applied where they will be most effective. Sometimes a boundary is defined by people, information, and information technology associated with one physical location.

**Implications:** Create a security architecture or design. &nbsp;




**Compartmentalise** 
----------------------

**Statement:** Sub-systems will be partitioned logically and isolated using physical devices and/or security controls.

**Rationale:** In accordance with the minimise attack surface and Defence in Depth principles, this compartmentalise principle keeps a sub-system, or logically grouped set of sub-systems, relatively self-contained such that compromise of one will not imply the compromise of another.

**Implications:** Use defence in depth security principles in the security architecture. Sourcing of (sub)systems is easily possible when this principles is implemented correctly. Eliminate or minimize dependencies between subsystems. This can result in using other (generic) security services like a separate identification or authentication service.




**Compile with all warnings enabled** 
---------------------------------------

**Statement:** Compile with all warnings enabled, in pedantic mode, and use one or more modern static source code analyzers. All code must be compiled, from the first day of development, with all compiler warnings enabled at the compiler's most pedantic setting. All code must compile with these setting without warnings. All code must be checked on each build with at least one, but preferably more than one, state-of-the-art static source code analyzer and should pass the analyses with zero warnings.

**Rationale:** There are several very effective static source code analyzers on the market today, and quite a few freeware tools as well. There is no excuse for any serious software development effort not to make use of this technology. It should be considered routine practice, especially for critical software development. The rule of zero warnings applies even in cases where the compiler or the static analyzer gives an erroneous warning: if the compiler or the static analyzer gets confused, the code causing the confusion should be rewritten so that it becomes more trivially valid. Many have been caught in the assumption that a warning was likely invalid, only to realize much later that the report was in fact valid for less obvious reasons. Static analyzers originally had a bad reputation due to the limited capabilities of early versions (e.g., the early Unix tool lint). The early tools produced mostly invalid messages, but this is not the case for the current generation of commercial tools. The best static analyzers today are fast, and they produce selective and accurate messages.

**Implications:** Provide awareness trainings of developers continuously. &nbsp;




**Complete mediation** 
------------------------

**Statement:** Complete mediation

**Rationale:** Access rights are completely validated every time an access occurs. Systems should rely as little as possible on access decisions retrieved from a cache. Again, file permissions tend to reflect this model: the operating system checks the user requesting access against the file’s ACL. The technique is less evident when applied to email, which must pass through separately applied packet filters, virus filters, and spam detectors.

**Implications:** Document decisions regarding use of cached data for security services. Usability aspects should be taken into account with setting cache invalidation timers.




**Computer security is constrained by societal factors** 
----------------------------------------------------------

**Statement:** Computer Security is Constrained by Societal Factors.

**Rationale:** The ability of security to support the mission of an organization may be limited by various factors, such as social issues. For example, security and workplace privacy can conflict. Commonly, security is implemented on an IT system by identifying users and tracking their actions. However, expectations of privacy vary and can be violated by some security measures. (In some cases, privacy may be mandated by law.)

**Implications:** User awareness campaigns should be included in the security processes on regular basis. IT security measurements are a part of the total security system. Organization processes en policies are of great importance. &nbsp;




**Computer Security Requires a Comprehensive and Integrated Approach** 
------------------------------------------------------------------------

**Statement:** Computer Security Requires a Comprehensive and Integrated Approach

**Rationale:** Providing effective computer security requires a comprehensive approach that considers a variety of areas both within and outside of the computer security field. This comprehensive approach extends throughout the entire information life cycle. To work effectively, security controls often depend upon the proper functioning of other controls. Many such interdependencies exist. If appropriately chosen, managerial, operational,and technical controls can work together synergistically.

**Implications:** The effectiveness of security controls (also) depends on such factors as system management, legal issues, quality assurance, and internal and management controls. Computer security needs to work with traditional security disciplines including physical and personnel security.




**Computer Security Responsibilities and Accountability Should Be Made Explicit** 
-----------------------------------------------------------------------------------

**Statement:** Computer Security Responsibilities and Accountability Should Be Made Explicit

**Rationale:** The responsibility and accountability3 of owners, providers, and users of IT systems and other parties4 concerned with the security of IT systems should be explicit.5 The assignment of responsibilities may be internal to an organization or may extend across organizational boundaries.

**Implications:** Depending on the size of the organization, the computer security program may be large or small, even a collateral duty of another management official. However, even small organizations can prepare a document that states organization policy and makes explicit computer security responsibilities.




**Computer Security Should Be Cost-Effective** 
------------------------------------------------

**Statement:** Computer Security Should Be Cost-Effective.

**Rationale:** The costs and benefits of security should be carefully examined in both monetary and nonmonetary terms to ensure that the cost of controls does not exceed expected benefits. Security should be appropriate and proportionate to the value of and degree of reliance on the IT systems and to the severity, probability, and extent of potential harm. Requirements for security vary, depending upon the particular IT system.

**Implications:** Calculated the cost of damage against security measurements. Take notice of legal boundaries possible and lawsuits possible (for liability)  if no adequate security measurements are taken. Consider using proven generic OSS security services when applicable. &nbsp; &nbsp;




**Computer Security should be periodically reassessed** 
---------------------------------------------------------

**Statement:** Computer Security Should Be Periodically reassessed

**Rationale:** Computers and the environments in which they operate are dynamic. System technology and users, data and information in the systems, risks associated with the system, and security requirements are ever-changing. Many types of changes affect system security: technological developments (whether adopted by the system owner or available for use by others); connection to external networks; a change in the value or use of information; or the emergence of a new threat. In addition, security is never perfect when a system is implemented.

**Implications:** Implement security audits and pentest with your security control processes. &nbsp;




**Computer Security Supports the Mission of the Organization** 
----------------------------------------------------------------

**Statement:** Computer Security Supports the Mission of the Organization.

**Rationale:** The purpose of computer security is to protect an organization's valuable resources, such as information, hardware, and software. Through the selection and application of appropriate safeguards, security helps the organization's mission by protecting its physical and financial resources, reputation, legal position, employees, and other tangible and intangible assets.

**Implications:** IT Security should like all other IT services enable to business to run their processes. So an enabling service and not a disabler service.




**Data in transit protection** 
--------------------------------

**Statement:** Data in transit protection

**Rationale:** Consumer data transiting networks should be adequately protected against tampering and eavesdropping via a combination of network protection and encryption.

**Implications:** If this principle is not implemented, then the integrity or confidentiality of the data may be compromised whilst in transit.




**Data is always protected** 
------------------------------

**Statement:** Data is protected from unauthorized use and disclosure. In addition to the traditional aspects of data classification, this includes, but is not limited to, protection of per-decisional, sensitive, source selection-sensitive, and proprietary information.

**Rationale:** Open sharing of information and the release of information via relevant legislation must be balanced against the need to restrict the availability of classified, proprietary, and sensitive information. Existing laws and regulations require the safeguarding of security and the privacy of data, while permitting free and open access.

**Implications:** Aggregation of data, both classified and not, will create a large target requiring review and de-classification procedures to maintain appropriate control. Access to information based on a need-to-know policy will force regular reviews of the body of information. Security needs must be identified and developed at the data level, not the application level. Data security safeguards can be put in place to restrict access to "view only", or "never see". Sensitivity labeling of data for access to pre-decisional, decisional, classified, sensitive, or proprietary information must be determined. Security must be designed into data elements from the beginning; it cannot be added later. Systems, data, and technologies must be protected from unauthorized access and manipulation. Headquarters information must be safeguarded against inadvertent or unauthorized alteration, sabotage, disaster, or disclosure.




**Declare data objects at the smallest possible level of scope** 
------------------------------------------------------------------

**Statement:** Declare data objects at the smallest possible level of scope.

**Rationale:** Basic principle of data-hiding. Clearly if an object is not in scope, its value cannot be referenced or corrupted. Similarly, if an erroneous value of an object has to be diagnosed, the fewer the number of statements where the value could have been assigned; the easier it is to diagnose the problem. The rule discourages the re-use of variables for multiple, incompatible purposes, which can complicate fault diagnosis.

**Implications:** Data should always be declared at the start of the scope in which it is used: for file scope, the declarations go at the top of the source file (never in a header file); for function scope, the declaration goes at the top of the function body; for block scope, at the start of the block. This means that declarations should not be placed at random places in the code, e.g., that the point of first use. Data objects only used in one file should be declared file static.




**Defense in depth** 
----------------------

**Statement:** Defense in depth should be a key architecture and design principle.

**Rationale:** Multi-layered security controls and practices are better than single defense layer.

**Implications:** Do not trust on security measurements from preceding functions. Prepare for the worst possible scenario. Implement multiple defence mechanism. Create a security architecture or design and document the different layers of protection. If one security service fails the security system should still be resistant against threads. Compartmentalize and work with secure boundaries for information flows.




**Design and implement audit mechanisms** 
-------------------------------------------

**Statement:** Design and implement audit mechanisms to detect unauthorized use and to support incident investigations.

**Rationale:** Organizations should monitor, record, and periodically review audit logs to identify unauthorized use and to ensure system resources are functioning properly. In some cases, organizations may be required to disclose information obtained through auditing mechanisms to appropriate third parties.

**Implications:** Audit logs must be protected against manipulation. (online/offline). All audit records should have a correct time stamp. Unified time service is needed for a secure audit service. Integrity of the audit system must be implemented. &nbsp;




**Design and operate an IT system to limit damage and to be resilient in response.** 
--------------------------------------------------------------------------------------

**Statement:** Design and operate an IT system to limit damage and to be resilient in response.

**Rationale:** Information systems should be resistant to attack, should limit damage, and should recover rapidly when attacks do occur. The principle suggested here recognizes the need for adequate protection technologies at all levels to ensure that any potential cyber attack will be countered effectively.

**Implications:** Defence in depth measurement Compartmentalize IT building blocks. &nbsp; &nbsp;




**Design for secure updates** 
-------------------------------

**Statement:** Design for secure updates

**Rationale:** All updates for a system must be verified. The source of the update must be known and the integrity must be verified. It is easier to upgrade small pieces of a system than huge blobs. Doing so ensures that the security implications of the upgrade are well understood and controlled.

**Implications:** Verify the integrity and provenance of upgrade packages. Make use of code signing and signed manifests to ensure that the system only consumes patches and updates of trusted origin. E.g. use secure hashing (sha). &nbsp;




**Design for security properties changing over time** 
-------------------------------------------------------

**Statement:** Design for security properties changing over time

**Rationale:** The migration of previous users (and/or the correct coexistence of the local and remote users) would need to happen in a way that does not compromise security.

**Implications:** Make security design modular and flexible from the start.




**Design reviews** 
--------------------

**Statement:** All architectures and designs must be reviewed. Minimal on security aspects and potential risks. Also to determine if all (security and privacy) principles and requirements are followed.

**Rationale:** Integrating security into the design phase saves money and time. Conduct a risk review with security professionals and threat model the application to identify key risks and to improve product and processes under development. This helps you integrate appropriate countermeasures into the design and architecture of the application. Improving architecture and design is by far the best option (time,cost etc) for dealing with security and privacy.

**Implications:** Organize or make use of a structured review process to benefit from review. SME (Subject Matter Experts) must be available for doing reviews. Reserve time to improve architectures and designs or to improve code. &nbsp;




**Design security to allow for regular adoption of new technology** 
---------------------------------------------------------------------

**Statement:** Design security to allow for regular adoption of new technology, including a secure and logical technology upgrade process.

**Rationale:** As mission and business processes and the threat environment change, security requirements and technical protection methods must be updated. IT-related risks to the mission/business vary over time and undergo periodic assessment.

**Implications:** 




**Develop and exercise contingency or disaster recovery procedures to ensure appropriate availability** 
---------------------------------------------------------------------------------------------------------

**Statement:** Develop and exercise contingency or disaster recovery procedures to ensure appropriate availability

**Rationale:** Continuity of operations plans or disaster recovery procedures address continuance of an organization’s operation in the event of a disaster or prolonged service interruption that affects the organization’s mission.

**Implications:** 




**Do not implement unnecessary security mechanisms.** 
-------------------------------------------------------

**Statement:** Do not implement unnecessary security mechanisms.

**Rationale:** Every security mechanism should support a security service or set of services, and every security service should support one or more security goals. Extra measures should not be implemented if they do not support a recognized service or security goal. Such mechanisms could add unneeded complexity to the system and are potential sources of additional vulnerabilities.

**Implications:** Only implement security measurements when needed.




**Don’t trust infrastructure** 
----------------------------------

**Statement:** Underlaying infrastructure cannot be assumed safe.

**Rationale:** Vulnerabilities are at hardware,firmwire, virtualization, middleware and application layers. To minimize data leakage risks trusting security of other objects should be prevented.

**Implications:** Sandbox model /Jericho model needed. Layered defense easily possible




**Don’t trust services (from others)** 
------------------------------------------

**Statement:** Services from others (departments, companies) should never (ever) be trusted.

**Rationale:** Security design should protect against services use of other layers or applications (also SAAS services). Systems or sub-systems outside the bounds of a receiving component must never be trusted implicitly.

**Implications:** Every input/output and given by external services must be validated. Authentication, authorization can be needed. Measurements to maintain availability when using services (input or output) requires strict measurements implemented.




**Earn or give, but never assume or trust** 
---------------------------------------------

**Statement:** Earn or give, but never assume or trust

**Rationale:** Offloading security functions from server to client exposes those functions to a much less trustworthy environment, which is one of the most common causes of security failures predicated on misplaced trust. Designs that place authorization, access control,enforcement of security policy, or embedded sensitive data in client software thinking that it won’t be discovered, modified, or exposed by clever users or malicious attackers are inherently weak. Such designs will often lead to compromises.

**Implications:** Make sure all data received from an untrusted client are properly validated before processing. When designing your systems, be sure to consider the context where code will be executed, where data will go, and where data entering your system comes from.




**Economy of mechanism** 
--------------------------

**Statement:** A simple design is easier to test and validate.

**Rationale:** Keep it simple to avoid risk. More is not always better. This means more components, more processes and more security measurements involved. One factor in evaluating a system's security is its complexity. If the design, implementation, or security mechanisms are highly complex, then the likelihood of security vulnerabilities increases. Simpler means less can go wrong. This well-known principle applies to any aspect of a system, but it deserves emphasis for protection mechanisms for this reason: design and implementation errors that result in unwanted access paths will not be noticed during normal use (since normal use usually does not include attempts to exercise improper access paths). &nbsp;

**Implications:** Avoid complexity. &nbsp;




**Ensure proper security in the shutdown or disposal of a system** 
--------------------------------------------------------------------

**Statement:** Ensure proper security in the shutdown or disposal of a system

**Rationale:** Although a system may be powered down, critical information still resides on the system and could be retrieved by an unauthorized user or organization. Access to critical information systems must be controlled at all times.

**Implications:** At the end of a system’s life-cycle, system designers should develop / design procedures to dispose of an information system’s assets in a proper and secure fashion. Procedures must be implemented to ensure system hard drives, volatile memory, and other media are purged to an acceptable level and do not retain residual information.




**Ensure that developers are trained in how to develop secure software.** 
---------------------------------------------------------------------------

**Statement:** Ensure that developers are trained in how to develop secure software.

**Rationale:** It is unwise to assume that developers know how to develop secure software. Therefore, ensure that developers are adequately trained in the development of secure software before developing the system. This includes application of engineering disciplines to design, development, configuration control, and integration and testing.

**Implications:** Training cost (permanent) for all staff involved in maintaining the IT assets of a company.




**Establish a sound security policy as the“foundation” for design.** 
--------------------------------------------------------------------------

**Statement:** Establish a sound security policy as the “foundation” for design.

**Rationale:** A security policy is an important document to develop while designing an information system. The security policy begins with the organization’s basic commitment to information security formulated as a general policy statement. The policy is then applied to all aspects of the system design or security solution. The policy identifies security goals (e.g., confidentiality, integrity, availability, accountability, and assurance) the system should support, and these goals guide the procedures, standards and controls used in the IT security architecture design. The policy also should require definition of critical assets, the perceived threat, and security-related roles and responsibilities.

**Implications:** A security architecture or security design should be based on requirements that are derived from the policies defined or directly of the policies. &nbsp;




**Establish secure defaults** 
-------------------------------

**Statement:** Establish secure defaults when system goes in error or exception status, or at default startup.

**Rationale:** Secure defaults lower the risk of bad configurations.

**Implications:** Security design principles and requirements must be implemented at first release. Installation of software without safe defaults is not possible. Secure defaults must be determined and configured. Secure defaults must be regularly tested




**External interface protection** 
-----------------------------------

**Statement:** External interface protection

**Rationale:** All external or less trusted interfaces of the service should be identified and have appropriate protections to defend against attacks through them. If this principle is not implemented, interfaces could be subverted by attackers in order to gain access to the service or data within it.

**Implications:** 




**Fail Safe Defaults** 
------------------------

**Statement:** Fail Safe Defaults

**Rationale:** A mechanism that, in the event of failure, responds in a way that will cause no harm, or at least a minimum of harm, to other devices or danger to personnel.

**Implications:** Stress under load and hard failure situations must be incorporated in the security test suite. Default system configuration at start-up is secure.




**Fail-safe default settings for security and access** 
--------------------------------------------------------

**Statement:** Fail-safe default settings for security and access. So in case of error security should not be compromised.

**Rationale:** In computing systems, the save default is generally “no access” so that the system must specifically grant access to resources. Most file access permissions work this way, though Windows also provides a “deny” right. Windows access control list (ACL) settings may be inherited, and the “deny” right gives the user an easy way to revoke a right granted through inheritance. However, this also illustrates why “default deny” is easier to understand and implement, since it’s harder to interpret a mixture of “permit” and “deny” rights.

**Implications:** 




**Formulate security measures to address multiple overlapping information domains** 
-------------------------------------------------------------------------------------

**Statement:** Formulate security measures to address multiple overlapping information domains.

**Rationale:** An information domain is a set of active entities (person, process, or devices) and their data objects. A single information domain may be subject to multiple security policies. A single security policy may span multiple information domains. An efficient and cost effective security capability should be able to enforce multiple security policies to protect multiple information domains without the need to separate (physically or logically) the information and respective information systems processing the data.

**Implications:** 




**Governance framework** 
--------------------------

**Statement:** A Governance framework is required for service providers of Cloud hosting.

**Rationale:** The service provider should have a security governance framework that coordinates and directs their overall approach to the management of the service and information within it. If this principle is not implemented, any procedural, personnel, physical and technical controls in place will not remain effective when responding to changes in the service and to threat and technology developments.

**Implications:** 




**HTTP header use** 
---------------------

**Statement:** HTTP header information is not relied on to make security decisions.

**Rationale:** HTTP headers can be manipulated very easily.

**Implications:** Test if software does not make security decisions based on HTTP headers. Perform e.g. security tests with manipulated headers. &nbsp;




**Identify and prevent common errors and vulnerabilities** 
------------------------------------------------------------

**Statement:** Identify and prevent common errors and vulnerabilities

**Rationale:** Many errors reoccur with disturbing regularity - errors such as buffer overflows, race conditions, format string errors, failing to check input for validity, and programs being given excessive privileges. Learning from the past will improve future results.

**Implications:** Use OWASP top 10 checklist Use proven security testtools that are regular updated.




**Identify potential trade-offs** 
-----------------------------------

**Statement:** Identify potential trade-offs between reducing risk and increased costs and decrease in other aspects of operational effectiveness.

**Rationale:** To meet stated security requirements, a systems designer, architect, or security practitioner will need to identify and address all competing operational needs. It may be necessary to modify or adjust (i.e., trade-off) security goals due to other operational requirements. In modifying or adjusting security goals, an acceptance of greater risk and cost may be inevitable.

**Implications:** Document all relevant design decisions within a maintained security architecture or design document. &nbsp;




**Identity and authentication** 
---------------------------------

**Statement:** Identity and authentication

**Rationale:** Access to all service interfaces (for consumers and providers) should be constrained to authenticated and authorised individuals. If this principle is not implemented, unauthorised changes to a consumer’s service, theft or modification of data, or denial of service may occur.

**Implications:** 




**Implement layered security (Ensure no single point of vulnerability).** 
---------------------------------------------------------------------------

**Statement:** Implement layered security (Ensure no single point of vulnerability).

**Rationale:** Security designs should consider a layered approach to address or protect against a specific threat or to reduce vulnerability. For example, the use of a packet-filtering router in conjunction with an application gateway and an intrusion detection system combine to increase the work-factor an attacker must expend to successfully attack the system.

**Implications:** 




**Implement least privilege** 
-------------------------------

**Statement:** Implement least privilege.

**Rationale:** The concept of limiting access, or "least privilege," is simply to provide no more authorizations than necessary to perform required functions. This is perhaps most often applied in the administration of the system. Its goal is to reduce risk by limiting the number of people with access to critical system security controls; i.e., controlling who is allowed to enable or disable system security features or change the privileges of users or programs. Best practice suggests it is better to have several administrators with limited access to security resources rather than one person with "super user" permissions.

**Implications:** 




**Implement tailored system security measures to meet organizational security goals.** 
----------------------------------------------------------------------------------------

**Statement:** Implement tailored system security measures to meet organizational security goals.

**Rationale:** In general, IT security measures are tailored according to an organization’s unique needs. While numerous factors, such as the overriding mission requirements, and guidance, are to be considered, the fundamental issue is the protection of the mission or business from IT security related, negative impacts.

**Implications:** 




**Isolate public access systems from mission critical resources** 
-------------------------------------------------------------------

**Statement:** Isolate public access systems from mission critical resources (e.g., data, processes, etc.).

**Rationale:** While the trend toward shared infrastructure has considerable merit in many cases, it is not universally applicable. In cases where the sensitivity or criticality of the information is high, organizations may want to limit the number of systems on which that data is stored and isolate them, either physically or logically. Physical isolation may include ensuring that no physical connection exists between an organization’s public access information resources and an organization’s critical information. When implementing logical isolation solutions, layers of security services and mechanisms should be established between public systems and secure systems responsible for protecting mission critical resources.

**Implications:** Isolation measurements must be tested regularly. An audit report from a third party is required (in case of cloud sourcing).




**Least common mechanism** 
----------------------------

**Statement:** Least common mechanism

**Rationale:** Users should not share system mechanisms except when absolutely necessary, because shared mechanisms may provide unintended communication paths or means of interference.

**Implications:** 




**Least privilege** 
---------------------

**Statement:** Least privilege

**Rationale:** Every program and user should operate while invoking as few privileges as possible. This is the rationale behind Unix “sudo” and Windows User Account Control, both of which allow a user to apply administrative rights temporarily to perform a privileged task.

**Implications:** This principle has impact on the system, software components, but also on procedures used. &nbsp;




**Limit the use of pointers** 
-------------------------------

**Statement:** Limit the use of pointers. Use no more than N levels of dereferencing (star operators) per expression. A strict value for N=1, but in some cases using N=2 can be justified. Pointer dereference operations may not be hidden in macro definitions or inside typedef declarations. The use of function pointers should be restricted to simple cases.

**Rationale:** Pointers are easily misused, even by experienced programmers. They can make it hard to follow or analyze the flow of data in a program, especially by tool-based static analyzers. Function pointers, similarly, can seriously restrict the types of checks that can be performed by static analyzers and should only be used if there is a strong justification for their use, and ideally alternate means are provided to assist tool-based checkers determine flow of control and function call hierarchies. For instance, if function pointers are used, it can become impossible for a tool to prove absence of recursion, so alternate guarantees would have to be provided to make up for this loss in analytical capabilities.

**Implications:** It should be possible for a static analyzer to determine in all cases which function is being called, if the call is made through a function pointer. It may be acceptable to allow cases where the number of possible functions that may be called is larger than one, provided it does not affect the precision of the code analysis itself. This means that it can depend on the capabilities of a specific static analyzer what liberties can be taken with the use of function pointers. Additionally, though, it is wise to keep function pointer use to a minimum, and to restrict to simple cases, to make sure that also humans can determine accurately and with modest effort which functions may be evoked.




**Limit the use of the preprocessor to file inclusion and simple macros** 
---------------------------------------------------------------------------

**Statement:** Limit the use of the preprocessor to file inclusion and simple macros. The use of the preprocessor must be limited to the inclusion of header files and simple macro definitions. Token pasting, variable argument lists (ellipses), and recursive macro calls are not permitted. All macros must expand into complete syntactic units. The use of conditional compilation directives should be restricted to the prevention of duplicate file inclusion in header files.

**Rationale:** The C preprocessor is a powerful obfuscation tool that can destroy code clarity and befuddle many text based checkers. The effect of constructs in unrestricted preprocessor code can be extremely hard to decipher, even with a formal language definition in hand. In a new implementation of the C preprocessor, developers often have to resort to using earlier implementations as the referee for interpreting complex defining language in the C standard. The rationale for the caution against conditional compilation is equally important. Note that with just ten conditional compilation directives, there could be up to 2^10 (i.e., 1024) possible versions of the code, each of which would have to be tested -- causing a significant increase in the required test effort.

**Implications:** Macros should only appear in header files, never in the source code itself. The #undef directive should not be used. Macros should never hide declarations, and they should not hide pointer dereference operations from the code. Macros should also never be used to redefine the language. The restriction of macro definitions to the definition of complete syntactic units means that all macro bodies must be enclosed in either round or curly braces. Compiler directives There should not be more #ifdef directives in a code base than there are headerfiles. Each use of compilation directives (other than the duplicate file inclusion prevention use) should be flagged by a tool-based checker and justified with a comment in the code.




**Logging secrets** 
---------------------

**Statement:** Private data (for example, passwords) is not logged.

**Rationale:** Protecting secure logs is expensive.

**Implications:** A clear message level must be built in to notify exactly what the cause of error is. Reduced risk profile on system logs.




**Minimize secrets** 
----------------------

**Statement:** Minimize secrets

**Rationale:** Secrets should be few and changeable, but they should also maximize entropy, and thus increase the attacker’s work factor. The simple principle is also true by itself, since each secret increases a system’s administrative burden.

**Implications:** 




**Minimize the system elements to be trusted.** 
-------------------------------------------------

**Statement:** Minimize the system elements to be trusted.

**Rationale:** Security measures include people, operations, and technology. Where technology is used, hardware, firmware, and software should be designed and implemented so that a minimum number of system elements need to be trusted in order to maintain protection.

**Implications:** 




**Open design** 
-----------------

**Statement:** Open design. The security of physical products, machines and systems should not depend on secrecy of the design and implementation.

**Rationale:** Baran (1964) argued persuasively in an unclassified RAND report that secure systems, including cryptographic systems, should have unclassified designs. This reflects recommendations by Kerckhoffs (1883) as well as Shannon’s maxim: “The enemy knows the system” (Shannon, 1948). Even the NSA, which resisted open crypto designs for decades, now uses the Advanced Encryption Standard to encrypt classified information.

**Implications:** 




**Operational security** 
--------------------------

**Statement:** Operational security

**Rationale:** The service provider should have processes and procedures in place to ensure the operational security of the service. processes and procedures in place to ensure the operational security of the service. If this principle is not implemented, the service can’t be operated and managed securely in order to impede, detect or prevent attacks against it.

**Implications:** 




**Personnel security** 
------------------------

**Statement:** Personnel security

**Rationale:** Service provider staff should be subject to personnel security screening and security education for their role. If this principle is not implemented, the likelihood of accidental or malicious compromise of consumer data by service provider personnel is increased.

**Implications:** 




**Protect information while being processed, in transit, and in storage.** 
----------------------------------------------------------------------------

**Statement:** Protect information while being processed, in transit, and in storage.

**Rationale:** The risk of unauthorized modification or destruction of data, disclosure of information, and denial of access to data while in transit should be considered along with the risks associated with data that is in storage or being processed. Therefore, system engineers, architects, and IT specialists should implement security measures to preserve, as needed, the integrity, confidentiality, and availability of data, including application software, while the information is being processed, in transit, and in storage.

**Implications:** 




**Provide assurance that the system is, and continues to be, resilient in the face of expected threats.** 
-----------------------------------------------------------------------------------------------------------

**Statement:** Provide assurance that the system is, and continues to be, resilient in the face of expected threats.

**Rationale:** Assurance is the grounds for confidence that a system meets its security expectations. These expectations can typically be summarized as providing sufficient resistance to both direct penetration and attempts to circumvent security controls. Good understanding of the threat environment, evaluation of requirement sets, hardware and software engineering disciplines, and product and system evaluations are primary measures used to achieve assurance. Additionally, the documentation of the specific and evolving threats is important in making timely adjustments in applied security and strategically supporting incremental security enhancements.

**Implications:** Security testing must be planned and performed on regular basis.




**Psychological acceptability** 
---------------------------------

**Statement:** Psychological acceptability

**Rationale:** This principle essentially requires the policy interface to reflect the user’s mental model of protection, and notes that users won’t specify protections correctly if the specification style doesn’t make sense to them.

**Implications:** 




**Reduce risk to an acceptable level.** 
-----------------------------------------

**Statement:** Reduce risk to an acceptable level.

**Rationale:** Risk is defined as the combination of (1) the likelihood that a particular threat source will exercise (intentionally exploit or unintentionally trigger) a particular information system vulnerability and (2) the resulting adverse impact on organizational operations, organizational assets, or individuals should this occur.

**Implications:** 




**Risk Based Approach to Security** 
-------------------------------------

**Statement:** Ensure that risks to confidentiality, integrity, and availability of information and technology systems are treated in a consistent and effective manner.

**Rationale:** Risk is the chance of something happening that will have an impact on company objectives and risk assessment is the overall process of risk identification, analysis, evaluation, and mitigation. Taking a risk based approach allows for the: better identification of threats to our projects and initiatives, more effective allocation and use of resources to manage those risks, and improved stakeholder confidence and trust as we better manage information and business risk.

**Implications:** The level and cost of information security controls to manage confidentiality, integrity, and availability risk must be appropriate and proportionate to the value of the information assets and the potential severity, probability, and extent of harm. Risks must identified so we are aware of what risks can occur, what existing controls are in place, the consequence and likelihood of the risk occurring, and a determination is made about how to treat those risks. Options for addressing information risk should be reviewed so that informed and documented decisions are made about the treatment of risk. Risk treatment involves choosing one or more options, which typically include: Accepting risk (by an appropriate team member signing off that he/she has accepted the risk and no further action is required) Avoiding risk (by an appropriate team member deciding not to pursue a particular initiative) Transferring risk (by an appropriate team member to an external entity such as insurance) Mitigating risk (by an appropriate team member by applying appropriate information security measures, e.g., access controls, network monitoring and incident management)




**Secure use of the service by the consumer** 
-----------------------------------------------

**Statement:** Secure use of the service by the consumer

**Rationale:** Consumers have certain responsibilities when using a cloud service in order for this use to remain secure, and for their data to be adequately protected. If this principle is not implemented, the security of cloud services and the data held within them can be undermined by poor use of the service by consumers.

**Implications:** 




**Security by Design** 
------------------------

**Statement:** Controls for the protection of confidentiality, integrity, and availability should be designed into all aspects of solutions from initiation, not as an afterthought. Security should also be designed into the business processes within which an IT system will be used.

**Rationale:** The implementation of protections for confidentiality, availability and integrity within information and systems at the end of a project is more expensive than including the security protections within the initial design of the project. Controls implemented at the end of a project are often less efficient and less integrated than those integrated within the core of the project. &nbsp;

**Implications:** Security is designed in as an integrated part of the system architecture, not added as an afterthought. Security mechanisms must span all tiers of the architecture, and must be scalable. All solutions, custom or commercial, must be tested for security. Possible areas of control which could be addressed and integrated include (but are not limited to): asset management and information classification; physical security; segregation of duties, protections against malicious code; backup; exchange of information; logging and monitoring; user access management; technical vulnerability management; compliance with legal requirements; and, information systems audit considerations.




**Sensitive Data** 
--------------------

**Statement:** Secrets are not stored in code.

**Rationale:** Storing secrets involves risk at all times.

**Implications:** Software code must be scanned on secrets (e.g. configuration details, passwords)




**Sensitive data must be identified** 
---------------------------------------

**Statement:** Sensitive data must be identified and it should be defined how the data is handled.

**Rationale:** Data sets do not exist only at rest, but in transit between components within a single system and between organizations. As data sets transit between systems, they may cross multiple trust boundaries. Identifying these boundaries and rectifying them with data protection policies is an essential design activity. Trust is just as tricky as data sensitivity, and the notion of trust enclaves is likely to dominate security conversations in the next decade.

**Implications:** Policy requirements and data sensitivity can change over time as the business climate evolves, as regulatory regimes change, as systems become increasingly interconnected, and as new data sources are incorporated into a system. Regularly revisiting and revising data protection policies and their design implications is essential.




**Separation between consumers** 
----------------------------------

**Statement:** Separation between consumers

**Rationale:** Separation should exist between different consumers of the service to prevent one malicious or compromised consumer from affecting the service or data of another.If this principle is not implemented, service providers can not prevent a consumer of the service affecting the confidentiality or integrity of another consumer’s data or service.

**Implications:** Sharing services between customers by Cloud Service Providers (CSP's) requires strict separation within the security model.




**Separation of privilege** 
-----------------------------

**Statement:** Separation of privilege

**Rationale:** A protection mechanism is more flexible if it requires two separate keys to unlock it, allowing for two-person control and similar techniques to prevent unilateral action by a subverted individual. The classic examples include dual keys for safety deposit boxes and the two-person control applied to nuclear weapons and Top Secret crypto materials. A protection mechanism is more flexible if it requires two separate keys to unlock it, allowing for two-person control and similar techniques to prevent unilateral action by a subverted individual. The classic examples include dual keys for safety deposit boxes and the two-person control applied to nuclear weapons and Top Secret crypto materials. Separation of privilege gives better data protection for internal fraud or internal hacks.

**Implications:** Security procedures are needed. Business Continuity and Disaster Recovery involve more effort. Reaction time in case of an incident can be reduced. &nbsp;




**Session lifetime** 
----------------------

**Statement:** Session lifetime is limited. Also for cookies.

**Rationale:** Security System performance

**Implications:** All transactions must be completed within max session time.




**Strive for operational ease of use.** 
-----------------------------------------

**Statement:** Strive for operational ease of use.

**Rationale:** The more difficult it is to maintain and operate a security control, the less effective that control is likely to be. Therefore, security controls should be designed to be consistent with the concept of operations and with ease-of-use as an important consideration.

**Implications:** 




**Strive for simplicity** 
---------------------------

**Statement:** Strive for simplicity

**Rationale:** The more complex the mechanism, the more likely it may possess exploitable flaws. Simple mechanisms tend to have fewer exploitable flaws and require less maintenance. Further, because configuration management issues are simplified, updating or replacing a simple mechanism becomes a less intensive process.

**Implications:** 




**Supply chain security** 
---------------------------

**Statement:** Supply chain security

**Rationale:** The service provider should ensure that its supply chain satisfactorily supports all of the security principles that the service claims to implement. If this principle is not implemented, it is possible that supply chain compromise can undermine the security of the service and affect the implementation of other security principles.

**Implications:** 




**Systems Owners Have Security Responsibilities Outside Their Own Organizations** 
-----------------------------------------------------------------------------------

**Statement:** Systems Owners Have Security Responsibilities Outside Their Own Organizations

**Rationale:** If a system has external users, its owners have a responsibility to share appropriate knowledge about the existence and general extent of security measures so that other users can be confident that the system is adequately secure. This does not imply that all systems must meet any minimum level of security, but does imply that system owners should inform their clients or users about the nature of the security.

**Implications:** Managers "should act in a timely, coordinated manner to prevent and to respond to breaches of security" to help prevent damage to others.2 However, taking such action should not jeopardize the security of systems.




**Treat security as an integral part of the overall system design.** 
----------------------------------------------------------------------

**Statement:** Treat security as an integral part of the overall system design.

**Rationale:** Security must be considered in information system design. Experience has shown it to be both difficult and costly to implement security measures properly and successfully after a system has been developed, so it should be integrated fully into the system life-cycle process. This includes establishing security policies, understanding the resulting security requirements, participating in the evaluation of security products, and finally in the engineering, design, implementation, and disposal of the system.

**Implications:** 




**Use an authentication mechanism that cannot be bypassed** 
-------------------------------------------------------------

**Statement:** Use a authentication mechanism that cannot be bypassed or tampered with.

**Rationale:** The ability to bypass an authentication mechanism can result in an unauthorized entity having access to a system or service that it shouldn’t.

**Implications:** It’s preferable to have a single method, component, or system responsible for authenticating users. Such a single mechanism can serve as a logical “choke point” that cannot be bypassed. Much as in code reuse, once a single mechanism has been determined to be correct, it makes sense to leverage it for all authentication.




**Use only Secure Protocols** 
-------------------------------

**Statement:** Only inherently secure protocols should be used. The protocol should not encapsulate another insecure protocol (IPSec / VPN etc.) The protocol should be capable of authenticating itself

**Rationale:** Insecure protocols introduce security risks than can be easily avoided.

**Implications:** Insecure Protocols (http for example) Only used where interaction with non-trusted environment essential. Protocol must be validated against application




**Use standard solutions** 
----------------------------

**Statement:** Existing security controls should be given preference over custom solutions

**Rationale:** Secure software is hard. The largest, most experienced and deep pocketed software developers in the world, both commercial and open source, are constantly patching security vulnerabilities in software that has been in the wild and hardened over many years. It is arguably implausible for developers of a particular system to invent and deliver a security solution that is as good as or better than an off-the-shelf solution. Add to that the need to fully and clearly document how the custom security solution works for maintainers of the software and new developers to comprehend, maintain and extend the solution and the cost of training up those resources.

**Implications:** 




**Use unique identities to ensure accountability** 
----------------------------------------------------

**Statement:** Use unique identities to ensure accountability

**Rationale:** An identity may represent an actual user or a process with its own identity, e.g., a program making a remote access. Unique identities are a required element in order to be able to: Maintain accountability and traceability of a user or process Assign specific rights to an individual user or process Provide for non-repudiation Enforce access control decisions Establish the identity of a peer in a secure communications path Prevent unauthorized users from masquerading as an authorized user.

**Implications:** 




**Where possible, base security on open standards for portability and interoperability.** 
-------------------------------------------------------------------------------------------

**Statement:** Where possible, base security on open standards for portability and interoperability.

**Rationale:** For security capabilities to be effective security program designers should make every effort to incorporate interoperability and portability into all security measures, including hardware and software, and implementation practices. In practice an open interface in OSS software (good documented) can be a good alternative to an open standard that lacks solid reference implementations and gives room to different ways of implementing external behaviour.

**Implications:** No all Commercial-off-the-shelf (COTS) software is usable. OSS solutions should provide open interfaces.