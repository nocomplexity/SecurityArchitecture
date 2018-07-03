
Integrating privacy requirements (GDPR)
========================================

This section outlines simple and effective ways for handling privacy requirements within your solution architecture. An important document that is input for privacy requirements is e.g. the EU General Data Protection Regulation (GDPR).


What is the GDPR?
^^^^^^^^^^^^^^^^^^^^^^^^^
Privacy, security, Internet  and IT systems are complex and form a toxic mix. Many things can and will go wrong. Often it is just a manner of time before real incidents happen. Since detection of privacy and security breaches is also non trivial to accomplish there is a great chance you will never known that your data is seen or copied by unauthorized persons. Privacy is a core value of individuals of democratic societies.

The new EU General Data Protection Regulation (GDPR) will become fully enforceable throughout the European Union . This regulation is an important change in data privacy regulation for every company who deals with EU individuals. 

Security and privacy can never be done correct afterwards. So you must design or redesign your information systems and take security and privacy as top requirements to reduce risks. 

What is personal information
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Personal data is any information that relates to an identified or identifiable living individual. Different pieces of information that can lead to the identification of a particular person, also constitute as personal data. 

This means that MAC addresses, IP addresses are data pieces that are defined as personal data under the GDPR. But since the GDPR is not specific on details you will not find terms like MAC address or IP address explicitly stated in the GDPR document.

Having an IP address and MAC address will not mean that you can easily identify a natural person. Most of the time information e.g. from ISPs or local network administrators is needed to determine the real individual behind an IP address.



Design rules for privacy design
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Design rules to do privacy by design good from the start are:

* No security = no privacy. Dead simple. You can never do privacy correct if security is hardly implemented.
* Use an open design. The security and privacy should not depend on secrecy of the design and implementation. This accounts for your core IT systems, but also for your control and management systems. So go for real open.
* Defensive data collection. Only collect data that is really needed. Limiting data collection and (long term)storage prevents risks on data leakage.
* Reduce IT complexity. Besides high cost for maintenance and change, complexity can lead to severe risks that can impact security, privacy and safety for humans. 

Storing privacy data
^^^^^^^^^^^^^^^^^^^^^^

Storing personal data or private data of others is always an issue.

The GDPR answer on how to store personal data is by using  “appropriate technical and organisational safeguards”.  So you are screwed. IT consultants, auditors and lawyers know this and will try to convince you that the only way to answer this question is to do extensive (and expensive) risks assessments. Solid technical knowledge on how data is really stored within systems, databases, clouds, is scarce. So you will be forced to invest a lot of time doing business and organizational risks assessments and spend less time on evaluating important technical risks that come with open or closed IT technologies.

The simplest and best answer to the question is: **Do not collect and store personal data.** 

On the technical solution level you will discover that you almost always need solution building blocks that will meet functionality like:

* Identity and access management
* (Secure)Data Storage
* Logging and auditing
* Encryption

You should use separate solution building blocks and make sure that when one will fail the personal data storage is still safe. So use principles like “Defense in depth” and compartmentalise among other crucial security principles.

The perfect simple secure “Data Storage” as simple technical answer for storing personal information does not exist. But smart is to standardize your IT landscape where possible by making use of reusable Solution Building Blocks (SBB’s). This prevents you from reinventing the wheel for every new GDPR challenge.

Encrypting data at rest (so storing data)  provides an effective protection against unauthorized or unlawful processing. It is especially effective to protect data against unauthorized access if the device storing the encrypted data is lost or stolen.

Below some tips for using (secure) solution building blocks for storing personal data, think of using:

* Make use of database encryption (All OSS databases support this perfectly, e.g. PostgreSQL, MariaDB , MongoDB)
* Make use of file system encryption or storage device encryption
* Make use of a secure Vault for the uttermost important secret information (Solid OSS implementations exist, like Hashicorp Vault )
* Make use a fancy new blockchain technology enabled storage protocol. But mind: You MUST known what you are doing, since (secure)storage of data on a blockchain does not make it private by and compliant for GDPR usage by default. 



GDPR tools
^^^^^^^^^^^^^

https://ico.org.uk/for-organisations/resources-and-support/data-protection-self-assessment/

Specific GDRP References
^^^^^^^^^^^^^^^^^^^^^^^^^

The only official EC site regarding the GDPR. Note that a lot of sites pretend to be official EC sites, but are setup by commercial companies!
https://ec.europa.eu/info/law/law-topic/data-protection_en 

The GDPR official text: http://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=EN 

