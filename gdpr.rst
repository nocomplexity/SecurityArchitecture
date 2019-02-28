
Integrating privacy requirements (GDPR)
========================================

This section outlines simple and effective ways for handling privacy requirements within your solution architecture. An important document that is input for privacy requirements is e.g. the EU General Data Protection Regulation (GDPR). 


What is the GDPR?
----------------------
Privacy, security, Internet  and IT systems are complex and form a toxic mix. Many things can and will go wrong. Often it is just a manner of time before real incidents happen. Since detection of privacy and security breaches is also non trivial to accomplish there is a great chance you will never known that your data is seen or copied by unauthorized persons. Privacy is a core value of individuals of democratic societies. 

**Tracking people without their knowledge, approval or a court order is just flat-out wrong.** The fact that it can be done is no excuse. Without adtech, and massive data collection of commercial companies, the EU’s GDPR (General Data Protection Regulation) would never have happened. The GDPR should put a hold to this practice. But the GDPR is no silver bullet. Many escapes are possible and without good security controls privacy can not exist.

The new EU General Data Protection Regulation (GDPR) will become fully enforceable throughout the European Union . This regulation is an important change in data privacy regulation for every company who deals with EU individuals. 

Security and privacy can never be done correct afterwards. So you must design or redesign your information systems and take security and privacy as top requirements to reduce risks. 

What is personal information
----------------------------------

Personal data is any information that relates to an identified or identifiable living individual. Different pieces of information that can lead to the identification of a particular person, also constitute as personal data. 

This means that MAC addresses, IP addresses are data pieces that are defined as personal data under the GDPR. But since the GDPR is not specific on details you will not find terms like MAC address or IP address explicitly stated in the GDPR document.

Having an IP address and MAC address will not mean that you can easily identify a natural person. Most of the time information e.g. from ISPs or local network administrators is needed to determine the real individual behind an IP address.



Design rules for privacy design
-----------------------------------

Design rules to do privacy by design good from the start are:

* No security = no privacy. Dead simple. You can never do privacy correct if security is hardly implemented.
* Use an open design. The security and privacy should not depend on secrecy of the design and implementation. This accounts for your core IT systems, but also for your control and management systems. So go for real open.
* Defensive data collection. Only collect data that is really needed. Limiting data collection and (long term)storage prevents risks on data leakage.
* Reduce IT complexity. Besides high cost for maintenance and change, complexity can lead to severe risks that can impact security, privacy and safety for humans. 

Storing privacy data
-----------------------

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

Permanent erasing of data
----------------------------

The GDPR introduces a right for individuals to have personal data erased. This right to erasure is also known as ‘the right to be forgotten’. This means that individuals can make a request for erasure verbally or in writing. This rule is outlined in article 17 of the GDPR, but the technical consequences and complexity that comes with this rule are not trivial to implement. And a clear answer for implementation is not present in the GDPR. So even deletion is risk based.

From a technical point of view real and permanent erasing of data is a real challenge!

Using a standard delete function from a database or operating system hardly will remove data. There are great ways to get data back after administrator errors or disasters. Deleted data is often still recoverable. So simply using a ‘delete’ doesn’t meet the GDPR compliance for erasure. Besides were do you start when deleting data? Data is often shared with suppliers, partners, resellers. But data is also transfered to various marketing companies or even sold. And data is also often stored on various on-line or off-line backups facilities. And do not forget to check if data that must be erased is present on log and audit files.

So to guarantee that data is deleted from all these different players is in practice hard to realize. Of course the key is not to share or sell gathered data in the first place, but this is not always possible. Some options are:

* If you have encrypted personal data an option for erasure is to use crypto-shredding. This is the practice of ‘deleting’ data by overwriting the encryption keys. However there can be consequences for data you do not want to delete if you are destroying your encryption keys.
* Use certified data erasure software. Data erasure software should comply with requirements to erase hidden areas, provide a defects log list and list bad sectors that could not be overwritten. Standards and rules for deleting data for various industries (e.g. health care and military) exist for many years already. Make reuse of this standards and rules to implementation of the GDPR easier. But erasing a data collection is  often easier that only deleting a single record.

**If data is or was available on the Internet, intended or unintended, is will be close to impossible to delete.**

Pseudonymization or Anonymization
-----------------------------------

Determining how to handle the GDPR is not straightforward when dealing with data masking.  A question relevant to comply with the GDPR is if you  should use:

* Anonymization or
* Pseudonymization

To mask personal data in your IT landscape.

According to the GDPR ‘pseudonymization’ means the processing of personal data in such a manner that the personal data can no longer be attributed to a specific data subject without the use of additional information, provided that such additional information is kept separately and is subject to technical and organizational measures to ensure that the personal data are not attributed to an identified or identifiable natural person. So Pseudonymization is a method to **substitute identifiable data with a reversible, consistent value.** So the weakness is that personal data is still there, only a bit more difficult to get if you have no information on the used pseudonymization rules.

Pseudonymization of personal data can reduce the risks to the data subjects concerned and help controllers and processors to meet GDPR obligations. But pseudonymization of data is in general a weak process to protect data privacy. Pseudonymization substitutes only the identity of the data subject in such a way that additional information is required to re-identify the data subject. A better approach to protect private data is to use data anonymization.

Data anonymization is the process of either **encrypting or removing** personally identifiable information from data sets, so that the private personal data remain anonymous. Real anonymization is irreversibly and destroys permanent any option of identifying the data subject.

Using pseudonymization introduces a large number of risks that are not present when using anomyzation. However in some use cases you can only use pseudonymization. But use it with care, since the technical and organizational risks involved with pseudonymization are significant.


Privacy Threat Modeling
-------------------------
To design systems with a low risk profile for privacy and security risks a good tool is to use thread modeling.

A privacy threat model is a way of looking at privacy risks in order to identify what threats to privacy (and security) exist for your situation. Some common privacy threats are:

-  Surveillance. Surveillance is the observation or monitoring of an individual’s communications or activities.
-  Stored Data Compromise. Systems that do not take adequate measures to secure data from unauthorized or inappropriate access expose a high risk for privacy.
-  Intrusion. Intrusion consists of invasive acts that disturb or interrupt one’s digital activities. E.g. network intrusion (on your digital communication) or video / audio intrusion to follow what you do.

Creating a dedicated privacy thread model is always recommended. Of course you should make use of general existing thread models (e.g. the STRIDE model) and tailor it for your specific situation. In essence creating a threat model is creating answers to the following questions:

- What do you want to protect? (E.g. What data, what kind of communication, what can be misused?)
- Who do you want to protect it from? (E.g. What people, which organizations, criminal actors etc.)
- How likely is it that you will need to protect it? (Your personal level of exposure to those threats.)
- How bad are the consequences if protection fails?
- How much trouble are you willing to go through in order to try to prevent against these threads? (E.g. cost/ money, time and convenience, loss of flexibility, etc )

Depending your domain, context and specific use case you should make use of thread models and measurements against common threads that are already invented by others. E.g. if you are a journalist, make use of thread models and tools that are already developed for you. And if you use an open model, make sure your improvements can again help others.


Protecting Privacy
-------------------

Despite the fact that the GDPR document starts with **"The protection of natural persons in relation to the processing of personal data is a fundamental right”** it is very hard for users and service provides to protect these rights. This because making it impossible to trace communication by third parties, including governments is very difficult. Most governments are still not very kind for persons with other principles. So there is a real need to make it possible to make tracing of communication impossible without throwing giving away all the benefits of current Internet communication technologies.

Using secure communication (e.g. VPN , HTTPS ) is almost a must have to be GDPR compliant. Encrypting data whilst it is being transferred from one device to another provides effective protection against interception of the communication by a third party whilst the data is in transfer.

There are some good FOSS tools available to protect your privacy if you have a hostile government and must protect your communication. E.g. take a look at Streisand, but a full list can be found in the section 'OSS Privacy Applications' 


Dealing with metadata
-----------------------

To meet the GDPR requirements you should be aware of the risk of exposing personal information by metadata in documents. So make use of metada anonymisation.

Metadata is data that consists of information that characterizes data (e.g. Word documents, pictures, music files, etc). In essence, metadata answers who, what, when, where, why, and how about every facet of the data that is being characterized. Metadata within a file can contain a lot of privacy related data.  Office documents like pdf or MSOffice automatically add author, company information and revision information(e.g. who changed what)  to documents and spreadsheets. Under the GDPR you are not by default allowed to disclose this metadata information on the web.

When you distribute information or publish information on the Internet you must check if metadata in document is still present and if you are allowed to expose this information. In most cases you do not want the metadata exposed. To solve this problem a lot of tools exist that claim to strip all metadata for you from Office Documents (MSWord, PDF, etc). However in most cases these tools work far from perfect and give you a false feeling of security. For examples, images embedded inside PDF documents may not be cleaned and images also contain metadata information.

From a GDPR perspective you must be sure that no metadata is present by accident in documents you publish. So before publishing documents you should convert documents to a format that do not contain any metadata at all: E.g. plain-text document. But be aware and very careful: every format can be watermarked, so also even plain text documents! E.g. by using white space steganography.  Steganography is the science of concealing messages in other messages. In this digital age with a lot of companies and governments following your communication, steganography provides still a good way for hiding messages.



GDPR tools
------------

https://ico.org.uk/for-organisations/resources-and-support/data-protection-self-assessment/

Specific GDRP References
---------------------------


The only official EC site regarding the GDPR. Note that a lot of sites pretend to be official EC sites, but are setup by commercial companies!
https://ec.europa.eu/info/law/law-topic/data-protection_en 

The GDPR official text: http://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=EN 

