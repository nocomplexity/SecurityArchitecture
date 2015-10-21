Privacy Principles
------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Access to Personal data</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">The organization provides individuals with access to their personal information for review or update.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">Comply with global or local regulations or legal constrains.</td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>Confirmation of individual's identity before access is given to personal information.</li>
<li>Personal information presented in understandable format.</li>
<li>Access provided in reasonable time frame and at a reasonable cost.</li>
<li>Statement of disagreement; the reason for denial should be explained to individuals in writing.</li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Collection Limitation Principle</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">There should be limits to the collection of personal data and any such data should be obtained by lawful and fair means and, where appropriate, with the knowledge or consent of the data subject. (Source:OECDprivacy.org, by Ben Gerber )</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">When collecting many personal data records this will have a significant impact on:
<ul>
<li>Risks</li>
<li>Costs</li>
</ul>
Collecting personal data means end-users trust you (you do no evil). The more data you collect the harder it will be to protect the data for other forms of usages in future.</td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>Make an architecture or design that is clear on what data objects are collected for what business process. Do not collect data with purpose of data mining based on vague use cases.</li>
<li>Make a data design for all data that is collected.</li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Collection of personal data</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">Personal information is only collected for the purposes identified in a notice presented to the users.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">Legal regulation (local, global)</td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>document and describe types of information collected and methods of collection</li>
<li>collection of information by fair and lawful means, including collection from third parties</li>
<li>inform individuals if information is developed or additional information is acquired</li>
</ul></td>
</tr>
</tbody>
</table>

| Name Principle   | Defensive data collection                                                                                                |
|------------------|--------------------------------------------------------------------------------------------------------------------------|
| **Statement**    | Limited data collected from users only for functionality needed.                                                         |
| **Rationale**    | Only collect data what is needed for performing functionality. Limiting data collection prevents risks on data leakage.  |
| **Implications** | De-identify where and when possible to reduce risk of privacy data concerns. Data must deleted when no longer necessary. |

| Name Principle   | Design reviews                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Statement**    | All architectures and designs must be reviewed. Minimal on security aspects and potential risks. Also to determine if all (security and privacy) principles and requirements are followed.                                                                                                                                                                                                                                                                     |
| **Rationale**    | Integrating security into the design phase saves money and time. Conduct a risk review with security professionals and threat model the application to identify key risks and to improve product and processes under development. This helps you integrate appropriate countermeasures into the design and architecture of the application. Improving architecture and design is by far the best option (time,cost etc) for dealing with security and privacy. |
| **Implications** | Organize or make use of a structured review process to benefit from review. SME (Subject Matter Experts) must be available for doing reviews. Reserve time to improve architectures and designs or to improve code.                                                                                                                                                                                                                                            |

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Disclosure to third parties</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">Personal information is disclosed to third parties only for the identified purposes and with implicit or explicit consent of the individual.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left"><ul>
<li>Communication with third parties should be made known to the individual</li>
<li>Information should only be disclosed to third parties that have equivalent agreements to protect personal</li>
<li>Information individuals should be aware of any new uses/purposes for the information the organization should take remedial action in response to misuse of personal information by a third party</li>
</ul></td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left">Make sure end-users can read , understand and agree with your privacy terms.</td>
</tr>
</tbody>
</table>

| Name Principle   | Don't trust infrastructure                                                                                                                                                          |
|------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Statement**    | Underlaying infrastructure cannot be assumed safe.                                                                                                                                  |
| **Rationale**    | Vulnerabilities are at hardware,firmwire, virtualization, middleware and application layers. To minimize data leakage risks trusting security of other objects should be prevented. |
| **Implications** | Sandbox model /Jericho model needed. Layered defense easily possible                                                                                                                |

| Name Principle   | Don't trust services (from others)                                                                                                                                                                                                      |
|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Statement**    | Services from others (departments, companies) should never (ever) be trusted.                                                                                                                                                           |
| **Rationale**    | Security design should protect against services use of other layers or applications (also SAAS services). Systems or sub-systems outside the bounds of a receiving component must never be trusted implicitly.                          |
| **Implications** | Every input/output and given by external services must be validated. Authentication, authorization can be needed. Measurements to maintain availability when using services (input or output) requires strict measurements implemented. |

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Individual Participation Principle</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">An individual should have the right to get clear insight on data collected that relates to him.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">Users should be informed on what is collected on request. In some countries this is a legal requirement for all companies collecting personal data.  </td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>User request should be handled within a reasonable time</li>
<li>At a minimal cost</li>
<li>Users should be informed on how data is protected, deleted and what data is shared with other companies.</li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Management Responsibility</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">The organization defines, documents, communicates and assigns accountability for its privacy policies and procedures.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">Management is responsible for organising processes needed to be compliant for privacy regulations and handling personal data within the company.</td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>privacy policies define and document all ten GAPP</li>
<li>review and approval of changes to privacy policies conducted by management</li>
<li>risk assessment process in place to establish a risk baseline and regularly identify new or changing risks to personal data</li>
<li>infrastructure and systems management takes into consideration impacts on personal privacy</li>
<li>privacy awareness training</li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Monitoring and enforcement</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">The organization monitors compliance with its privacy policies and procedures. It also has procedures in place to address privacy-related complaints and disputes.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"><ul>
<li>individuals should be informed on how to contact the organization with inquiries, complaints and disputes</li>
<li>formal process in place for inquires, complaints or disputes</li>
<li>each complaint is addressed and the resolution is documented for the individual</li>
<li>compliance with privacy policies, procedures, commitments and legislation is reviewed, documented and reported to management</li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Purpose Specification Principle</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">The purposes for which personal data are collected should be specified not later than at the time of data collection and the subsequent use limited to the fulfilment of those purposes or such others as are not incompatible with those purposes and as are specified on each occasion of change of purpose. (source: http://oecdprivacy.org/)</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left"></td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left">The purpose of personal data collection must be clearly defined in an architecture or design. This involves business, functional and IT designs.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Security for privacy</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">Personal information is protected against both physical and logical unauthorized access.</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left"><ul>
<li>privacy policies must address the security of personal information</li>
<li>information security programs must include administrative, technical and physical safeguards</li>
<li>logical access controls in place</li>
<li>restrictions on physical access</li>
<li>environmental safeguards</li>
<li>personal information protected when being transmitted (e.g. mail, internet, public or other non-secure networks)</li>
<li>security safeguards should be tested for effectiveness at least once annually</li>
</ul></td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"></td>
</tr>
</tbody>
</table>

| Name Principle   | Security Safeguards                                                                                                                                                          |
|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Statement**    | Personal data should be protected by reasonable security safeguards against such risks as loss or unauthorised access, destruction, use, modification or disclosure of data. |
| **Rationale**    | Personal data is valuable.                                                                                                                                                   |
| **Implications** | Security must be in place. Security control system must be operational. (prevent,detect, react etc)                                                                          |

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Name Principle</th>
<th align="left">Use Limitation Principle</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>Statement</strong></td>
<td align="left">Personal data should not be disclosed, made available or otherwise used for purposes other than those specified in accordance with a) with the consent of the data subject; or b) by the authority of law. (source: http://oecdprivacy.org/)</td>
</tr>
<tr class="even">
<td align="left"><strong>Rationale</strong></td>
<td align="left">Using personal data for other means than collected introduces extra risks and complexity for your security and privacy operations. Most of the time other use of data is not securely designed.</td>
</tr>
<tr class="odd">
<td align="left"><strong>Implications</strong></td>
<td align="left"></td>
</tr>
</tbody>
</table>


