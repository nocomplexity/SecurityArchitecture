Privacy Principles
=======================

EU GDPR privacy principles
----------------------------

The EU General Data Protection Regulation (GDPR).

The GDPR key principles are:

* Personal data shall be processed lawfully, fairly and in a transparent manner in relation to the data subject (‘lawfulness, fairness and transparency’);
* Personal data shall be collected for specified, explicit and legitimate purposes and not further processed in a manner that is incompatible with those purposes; further processing for archiving purposes in the public interest, scientific or historical research purposes or statistical purposes shall, in accordance with Article 89(1), not be considered to be incompatible with the initial purposes (‘purpose limitation’);
* Personal data shall be adequate, relevant and limited to what is necessary in relation to the purposes for which they are processed (‘data minimisation’);
* Personal data shall be accurate and, where necessary, kept up to date; every reasonable step must be taken to ensure that personal data that are inaccurate, having regard to the purposes for which they are processed, are erased or rectified without delay (‘accuracy’);
* Personal data shall be kept in a form which permits identification of data subjects for no longer than is necessary for the purposes for which the personal data are processed;
* Personal data may be stored for longer periods insofar as the personal data will be processed solely for archiving purposes in the public interest, scientific or historical research purposes or statistical purposes in accordance with Article 89(1) subject to implementation of the appropriate technical and organisational measures required by this Regulation in order to safeguard the rights and freedoms of the data subject (‘storage limitation’);
* Personal data shall be processed in a manner that ensures appropriate security of the personal data, including protection against unauthorised or unlawful processing and against accidental loss, destruction or damage, using appropriate technical or organisational measures (‘integrity and confidentiality’).
* The controller shall be responsible for, and be able to demonstrate compliance (‘accountability’).

The ‘controller’ is the natural or legal person, public authority, agency or other body which, alone or jointly with others, determines the purposes and means of the processing of personal data.

Since visuals are easier to handle than text, a simple visual of the GDPR visuals here below:

.. image:: /Images/gdpr-principles.png
   :width: 600px 
   :alt: GDPR principles
   :align: center 

Data protection should be done according by the GDPR by design and by default. However the implementation challenge is: What are appropriate technical and/or organisational measurements for protecting private data? And the good news is: If you are processing privacy related data you decide what appropriate is. The only requirement is that you must document your decisions  so that you can justify your reasoning.

The risk with the GDPR is that your IT Cost will rise, due to the fact that solid quality standardized reusable open solutions are not offered by most commercial IT vendors and consultancy companies. So make use of the OSS solution building blocks that are outlined in this reference architecture.


Other privacy principles
-------------------------

Long before the EU GDPR principles was released many good privacy principles already existed. Below some important principles that are usable in many privacy architectures.


**Access to Personal data** 
-----------------------------

**Statement:** The organization provides individuals with access to their personal information for review or update.

**Rationale:** Comply with global or local regulations or legal constrains.

**Implications:** confirmation of individual’s identity before access is given to personal information personal information presented in understandable format access provided in reasonable time frame and at a reasonable cost statement of disagreement; the reason for denial should be explained to individuals in writing


**Data anomyzation**
----------------------

**Statement:** The use of data anomyzation is preferred when dealing with private data.
**Rationale:** Easier to comply with GDPR.
**Implication:** Only for business processes where data anomyzation is not possible data pseudonymization should be considered.


**Collection Limitation Principle** 
-------------------------------------

**Statement:** There should be limits to the collection of personal data and any such data should be obtained by lawful and fair means and, where appropriate, with the knowledge or consent of the data subject. (Source:OECDprivacy.org)



**Collection of personal data** 
---------------------------------

**Statement:** Personal information is only collected for the purposes identified in a notice presented to the users.

**Rationale:** Legal regulation (local, global)

**Implications:** document and describe types of information collected and methods of collection collection of information by fair and lawful means, including collection from third parties inform individuals if information is developed or additional information is acquired




**Defensive data collection** 
-------------------------------

**Statement:** Limited data collected from users only for functionality needed.

**Rationale:** Only collect data what is needed for performing functionality. Limiting data collection prevents risks on data leakage.

**Implications:** De-identify where and when possible to reduce risk of privacy data concerns. Data must deleted when no longer necessary.




**Design reviews** 
--------------------

**Statement:** All architectures and designs must be reviewed. Minimal on security aspects and potential risks. Also to determine if all (security and privacy) principles and requirements are followed.

**Rationale:** Integrating security into the design phase saves money and time. Conduct a risk review with security professionals and threat model the application to identify key risks and to improve product and processes under development. This helps you integrate appropriate countermeasures into the design and architecture of the application. Improving architecture and design is by far the best option (time,cost etc) for dealing with security and privacy.

**Implications:** Organize or make use of a structured review process to benefit from review. SME (Subject Matter Experts) must be available for doing reviews. Reserve time to improve architectures and designs or to improve code. &nbsp;




**Disclosure to third parties** 
---------------------------------

**Statement:** Personal information is disclosed to third parties only for the identified purposes and with implicit or explicit consent of the individual.

**Rationale:** Communication with third parties should be made known to the individual Information should only be disclosed to third parties that have equivalent agreements to protect personal Information individuals should be aware of any new uses/purposes for the information the organization should take remedial action in response to misuse of personal information by a third party



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




**Individual Participation Principle** 
----------------------------------------

**Statement:** An individual should have the right: a) to obtain from a data controller, or otherwise, confirmation of whether or not the data controller has data relating to him; b) to have communicated to him, data relating to him i) within a reasonable time; ii) at a charge, if any, that is not excessive; iii) in a reasonable manner; and iv) in a form that is readily intelligible to him; c) to be given reasons if a request made under subparagraphs (a) and (b) is denied, and to be able to challenge such denial; and d) to challenge data relating to him and, if the challenge is successful to have the data erased, rectified, completed or amended.



**Management Responsibility** 
-------------------------------

**Statement:** The organization defines, documents, communicates and assigns accountability for its privacy policies and procedures.

**Rationale:** Management is responsible for organising processes needed to be compliant for privacy regulations and handling personal data within the company.

**Implications:** privacy policies define and document all ten GAPP review and approval of changes to privacy policies conducted by management risk assessment process in place to establish a risk baseline and regularly identify new or changing risks to personal data infrastructure and systems management takes into consideration impacts on personal privacy privacy awareness training




**Monitoring and enforcement** 
--------------------------------

**Statement:** The organization monitors compliance with its privacy policies and procedures. It also has procedures in place to address privacy-related complaints and disputes.

**Rationale:** 

**Implications:** individuals should be informed on how to contact the organization with inquiries, complaints and disputes formal process in place for inquires, complaints or disputes each complaint is addressed and the resolution is documented for the individual compliance with privacy policies, procedures, commitments and legislation is reviewed, documented and reported to management




**Purpose Specification Principle** 
-------------------------------------

**Statement:** The purposes for which personal data are collected should be specified not later than at the time of data collection and the subsequent use limited to the fulfilment of those purposes or such others as are not incompatible with those purposes and as are specified on each occasion of change of purpose. (source: http://oecdprivacy.org/)





**Security for privacy** 
--------------------------

**Statement:** Personal information is protected against both physical and logical unauthorized access.

**Rationale:** privacy policies must address the security of personal information information security programs must include administrative, technical and physical safeguards logical access controls in place restrictions on physical access environmental safeguards personal information protected when being transmitted (e.g. mail, internet, public or other non-secure networks) security safeguards should be tested for effectiveness at least once annually



**Security Safeguards** 
-------------------------

**Statement:** Personal data should be protected by reasonable security safeguards against such risks as loss or unauthorised access, destruction, use, modification or disclosure of data.

**Rationale:** Personal data is valuable.

**Implications:** Security must be in place. Security control system must be operational. (prevent,detect, react etc) &nbsp;




**Use Limitation Principle** 
------------------------------

**Statement:** Personal data should not be disclosed, made available or otherwise used for purposes other than those specified in accordance with Paragraph 9 except: a) with the consent of the data subject; or b) by the authority of law. (source: http://oecdprivacy.org/)

