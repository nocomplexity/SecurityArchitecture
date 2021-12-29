# STRIDE 

STRIDE is currently the most mature threat-modeling method. 

STRIDE is a model for identifying computer security threats developed by Praerit Garg and Loren Kohnfelder at Microsoft. It provides a mnemonic for security threats in six categories.

The threats are:

* Spoofing
*    Tampering
*    Repudiation
*    Information disclosure (privacy breach or data leak)
*    Denial of service
*    Elevation of privilege

( [source Wikipedia, support it!](https://en.wikipedia.org/wiki/STRIDE_(security)) )

<table class="MsoNormalTable" cellspacing="0" cellpadding="0" border="0">
<tbody>
<tr style="mso-yfti-irow: 0; mso-yfti-firstrow: yes;">
<td class="x-hidden-focus" style="border-right: white 1pt solid; border-top: white 1pt solid; background: #4f81bd; border-left: white 1pt solid; border-bottom: white 3pt solid; padding: 0.05in 0.1in 0.05in 0.1in;" width="189" valign="top">
<p class="MsoPlainText x-hidden-focus" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Property </span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: white 1pt solid; background: #4f81bd; border-left: #f0f0f0; border-bottom: white 3pt solid; padding: 0.05in 0.1in 0.05in 0.1in;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Threat </span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: white 1pt solid; background: #4f81bd; border-left: #f0f0f0; border-bottom: white 3pt solid; padding: 0.05in 0.1in 0.05in 0.1in;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Definition </span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: white 1pt solid; background: #4f81bd; border-left: #f0f0f0; border-bottom: white 3pt solid; padding: 0.05in 0.1in 0.05in 0.1in;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Example </span></p>
</td>
</tr>
<tr style="mso-yfti-irow: 1;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Authentication</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>S</b>poofing</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;">Impersonating something or someone else. </span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;">Pretending to be any of billg, microsoft.com or ntdll.dll </span></span></p>
</td>
</tr>
<tr style="mso-yfti-irow: 2;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Integrity</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>T</b>ampering</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Modifying data or code</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Modifying a DLL on disk or DVD, or a packet as it traverses the LAN.</span></p>
</td>
</tr>
<tr style="mso-yfti-irow: 3;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Non-repudiation</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>R</b>epudiation</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Claiming to have not performed an action.</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">“I didn’t send that email,” “I didn’t modify that file,” “I <i>certainly</i> didn’t visit that web site, dear!”</span></p>
</td>
</tr>
<tr style="mso-yfti-irow: 4;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Confidentiality</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>I</b>nformation Disclosure</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Exposing information to someone not authorized to see it</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Allowing someone to read the Windows source code; publishing a list of customers to a web site.</span></p>
</td>
</tr>
<tr style="height: 69.8pt; mso-yfti-irow: 5;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Availability</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>D</b>enial of Service</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Deny or degrade service to users</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #d0d8e8; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Crashing Windows or a web site, sending a packet and absorbing seconds of CPU time, or routing packets into a black hole.</span></p>
</td>
</tr>
<tr style="height: 55.45pt; mso-yfti-irow: 6; mso-yfti-lastrow: yes;">
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: white 1pt solid; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="189" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Authorization</span></p>
</td>
<td class="" style="border-right: white 1pt solid; padding-right: 5.4pt; border-top: #f0f0f0; padding-left: 5.4pt; border-left-color: #f0f0f0; background: #e9edf4; padding-bottom: 0in; border-bottom: white 1pt solid;" width="147" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-size: medium;"><span style="font-family: calibri;"><b>E</b>levation of Privilege</span></span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="197" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Gain capabilities without proper authorization</span></p>
</td>
<td class="" style="border-right: white 1pt solid; border-top: #f0f0f0; background: #e9edf4; border-left: #f0f0f0; border-bottom: white 1pt solid; padding: 0.75pt 5.4pt 0in 5.4pt;" width="395" valign="top">
<p class="MsoPlainText" style="margin: 0in 0in 0pt;"><span style="font-family: calibri; font-size: medium;">Allowing a remote internet user to run commands is the classic example, but going from a limited user to admin is also EoP.</span></p>
</td>
</tr>
</tbody>
</table>

([source Microsoft](https://www.microsoft.com/security/blog/2007/09/11/stride-chart/) )