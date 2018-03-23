OSS Security Applications
============================


**411 Managing Security Alerts** 
-----------------------------------
**SBB Description:** An Alert Management Web Application.
411 is a Search scheduler.Configure Searches to periodically run against a variety of data sources. You can define a custom pipeline of Filters to manipulate any generated Alerts and forward them to multiple Targets.
An alert management interface.Review and manage Alerts through the web interface. You can apply Renderers to alerts to enrich them with additional metadata.

Typical Use cases for 411:

You want to detect when certain log lines show up in ES.
You want to detect when a Graphite metric changes.
You want to detect when a server stops responding
You want to manage alerts through a simple workflow. And much more!

**SBB License:** MIT License

**Core Technology:** PHP

**Project URL:** 

**Source Location:** https://github.com/etsy/411





**American fuzzy lop** 
------------------------
**SBB Description:** American fuzzy lop is a security-oriented fuzzer that employs a novel type of compile-time instrumentation and genetic algorithms to automatically discover clean, interesting test cases that trigger new internal states in the targeted binary. This substantially improves the functional coverage for the fuzzed code.
These tool can be very productive in determining security flaws: The famous SSL Heartbleed bug was found in record time using this software. See https://blog.hboeck.de/archives/868-How-Heartbleed-couldve-been-found.html.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** http://lcamtuf.coredump.cx/afl/

**Source Location:** http://lcamtuf.coredump.cx/afl/releases/





**Bokken (Open Source Reverse Code Engineering)** 
---------------------------------------------------
**SBB Description:** Bokken is an Open Source Reverse Code Engineering tool.
Bokken is a GUI for the Pyew and Radare projects so it offers almost all the same features that Pyew has and and some of the Radare&#8217;s ones. It&#8217;s intended to be a basic disassembler, mainly, to analyze malware and vulnerabilities.
Currently Bokken is neither an hexadecimal editor nor a full featured disassembler YET, so it should not be used for deep code analysis or to try to modify files with it.
Bokken has the ability to detect and analyze PE/Elf/mach0 files so, when one of those file formats is detected, the GUI shows all the information found on the analysis and offers many additional options to study the file.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python

**Project URL:** http://bokken.re

**Source Location:** https://inguma.eu/projects/bokken/repository





**Bosun** 
-----------
**SBB Description:** Bosun is an open-source, MIT licensed, monitoring and alerting system by Stack Exchange. It has an expressive domain specific language for evaluating alerts and creating detailed notifications. It also lets you test your alerts against history for a faster development experience.
Collecting metrics about our systems is fun but what makes a monitoring system useful is alerting when anomalies arise. This is the real strength of Bosun.
Bosun encourages a particular workflow that makes it easy to design, test, and deploy an alert. If you look at the top of the Bosun display, the tabs include Items, Graph, Expression, Rule, and Test config in left-to-right order; that reflects the phases you go through as you create an alert. In general, first you’ll select an item (metric) that is the basis of the alert.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** GO

**Project URL:** http://bosun.org/

**Source Location:** https://github.com/bosun-monitor/bosun





**Bro** 
---------
**SBB Description:** Bro is a powerful network analysis framework. Bro is a passive, open-source network traffic analyzer. It is primarily a security monitor that inspects all traffic on a link in depth for signs of suspicious activity. Bro supports a wide range of traffic analysis tasks even outside of the security domain, including performance measurements and helping with trouble-shooting.
The most immediate benefit that a site gains from deploying Bro is an extensive set of log files that record a network’s activity in high-level terms. These logs include not only a comprehensive record of every connection seen on the wire, but also application-layer transcripts such as, e.g., all HTTP sessions with their requested URIs, key headers, MIME types, and server responses; DNS requests with replies; SSL certificates; key content of SMTP sessions; and much more. By default, Bro writes all this information into well-structured tab-separated log files suitable for post-processing with external software. Users can however also chose from a set of alternative output formats and backends to interface directly with, e.g., external databases.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C 

**Project URL:** https://www.bro.org

**Source Location:** https://github.com/bro





**Data Seal** 
---------------
**SBB Description:** Data Seal is a lightweight, UELMA-compliant data authentication service.
Data Seal is a project of U.S. Open Data to provide a system where open data released by governments can be authenticated by end users—whether or not the data was most recently downloaded from the official source.
Government data releases need to abide by local laws (for example, the District of Columbia Official Code) and should also abide by the Uniform Electronic Legal Material Act (UELMA). Part of the UELMA provisions state that “legal material be…authenticated, by providing a method to determine that it is unaltered”.
Data Seal provides agencies with a web-based interface to provide this functionality.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Django/Python

**Project URL:** https://github.com/unitedstates/data-seal/wiki

**Source Location:** https://github.com/unitedstates/data-seal





**Datastream** 
----------------
**SBB Description:** An open-source framework for real-time anomaly detection using Python, ElasticSearch and Kiban. Also uses scikit-learn.

&#160;

**SBB License:** Apache License 2.0

**Core Technology:** Python

**Project URL:** https://github.com/MentatInnovations/datastream.io

**Source Location:** https://github.com/MentatInnovations/datastream.io





**Fail2ban** 
--------------
**SBB Description:** Fail2ban scans log files (e.g. /var/log/apache/error_log) and bans IPs that show the malicious signs &#8212; too many password failures, seeking for exploits, etc. Generally Fail2Ban is then used to update firewall rules to reject the IP addresses for a specified amount of time, although any arbitrary other action (e.g. sending an email) could also be configured. Out of the box Fail2Ban comes with filters for various services (apache, courier, ssh, etc).

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python

**Project URL:** https://www.fail2ban.org/wiki/index.php/Main_Page

**Source Location:** https://github.com/fail2ban





**FIDO (Fully Integrated Defense Operation)** 
-----------------------------------------------
**SBB Description:** FIDO (Fully Integrated Defense Operation &#8211; apologies to the FIDO Alliance for acronym collision) is developed by NetFlix and is now OSS. This system is for automatically analyzing security events and responding to security incidents.
The premise of FIDO is simple&#8230; each year companies are receiving an ever increasing amount of security related alerts. Instead of hiring more analyst to comb through the endless stream of alerts we automate the analysis to combat the barrage of information. Simply put, we integrate and then automate the manual human processes by codifying the logic and process used by threat analysts to provide consistent and reliable results.
The typical process for investigating security-related alerts is labor intensive and largely manual. To make the situation more difficult, as attacks increase in number and diversity, there is an increasing array of detection systems deployed and generating even more alerts for security teams to investigate.
FIDO is a NetFlix OSS project, see: http://techblog.netflix.com/2015/05/introducing-fido-automated-security.html

**SBB License:** Apache License 2.0

**Core Technology:** C# 

**Project URL:** https://github.com/Netflix/Fido/wiki

**Source Location:** https://github.com/Netflix/Fido





**GNUnet** 
------------
**SBB Description:** GNUnet is a mesh routing layer for end-to-end encrypted networking and a framework for distributed applications designed to replace the old insecure Internet protocol stack.
In other words, GNUnet provides a strong foundation of free software for a global, distributed network that provides security and privacy. Along with an application for secure publication of files, it has grown to include all kinds of basic applications for the foundation of a GNU internet.
GNUnet is an official GNU package.
The foremost goal of the GNUnet project is to become a widely used, reliable, open, non-discriminating, egalitarian, unfettered and censorship-resistant system of free information exchange. We value free speech above state secrets, law-enforcement or intellectual property. GNUnet is supposed to be an anarchistic network, where the only limitation for peers is that they must contribute enough back to the network such that their resource consumption does not have a significant impact on other users. GNUnet should be more than just another file-sharing network. The plan is to offer many other services and in particular to serve as a development platform for the next generation of decentralized Internet protocols.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** https://gnunet.org/

**Source Location:** https://gnunet.org/svn/





**Gryffin** 
-------------
**SBB Description:** Gryffin is a large scale web security scanning platform. Created by Yahoo, and since September 2015 available as open source.
It is not yet another scanner. It was written to solve two specific problems with existing scanners: coverage and scale. Better coverage translates to fewer false negatives. Inherent scalability translates to capability of scanning, and supporting a large elastic application infrastructure. Simply put, the ability to scan 1000 applications today to 100,000 applications tomorrow by straightforward horizontal scaling.

**SBB License:** MIT License

**Core Technology:** Go

**Project URL:** https://github.com/yahoo/gryffin

**Source Location:** https://github.com/yahoo/gryffin





**Hammertime** 
----------------
**SBB Description:** Hammertime: a software suite for testing, profiling and simulating the rowhammer DRAM defect.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python / C

**Project URL:** https://github.com/vusec/hammertime

**Source Location:** https://github.com/vusec/hammertime





**Hashcat** 
-------------
**SBB Description:** hashcat is the world&#8217;s fastest and most advanced password recovery utility, supporting five unique modes of attack for over 200 highly-optimized hashing algorithms. hashcat currently supports CPUs, GPUs, and other hardware accelerators on Linux, Windows, and macOS, and has facilities to help enable distributed password cracking.

**SBB License:** MIT License

**Core Technology:** C

**Project URL:** https://hashcat.net/hashcat/

**Source Location:** https://github.com/hashcat/hashcat





**Httpswatch** 
----------------
**SBB Description:** Test tool and site to verify if HTTPS is used as should be for website.
&#160;

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python

**Project URL:** https://httpswatch.com

**Source Location:** https://github.com/benjaminp/httpswatch





**Kali** 
----------
**SBB Description:** Kali is the most complete &#8216;Penetration Testing Linux Distribution&#8217; around. Everything you need for penetration testing is collected, tested and made available on this linux distribution. Of course all tools are OSS.
The complete list of tools can be found here:http://tools.kali.org/tools-listing

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** N.A. (OSS Tool collection) 

**Project URL:** https://www.kali.org/

**Source Location:** http://git.kali.org/gitweb/





**Kismet** 
------------
**SBB Description:** Kismet is an 802.11 layer2 wireless network detector, sniffer, and intrusion detection system. Kismet will work with any wireless card which supports raw monitoring (rfmon) mode, and (with appropriate hardware) can sniff 802.11b, 802.11a, 802.11g, and 802.11n traffic. Kismet also supports plugins which allow sniffing other media such as DECT.
Kismet identifies networks by passively collecting packets and detecting standard named networks, detecting (and given time, decloaking) hidden networks, and inferring the presence of non beaconing networks via data traffic. The great feature of Kismet is that this tool works working passively, so detection by IDS is prevented when scanning WLAN&#8217;s.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C++

**Project URL:** http://www.kismetwireless.net/

**Source Location:** https://www.kismetwireless.net/code/





**Libreswan** 
---------------
**SBB Description:** Libreswan is an IPsec implementation for Linux. Libreswan is a free software implementation of the most widely supported and standarized VPN protocol based on (&#8220;IPsec&#8221;) and the Internet Key Exchange (&#8220;IKE&#8221;).
&#160;

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** 

**Project URL:** https://libreswan.org/

**Source Location:** https://github.com/libreswan/libreswan





**Lightbulb** 
---------------
**SBB Description:** LightBulb is an open source python framework for auditing web applications firewalls.
Project created and started in 2016.

**SBB License:** MIT License

**Core Technology:** Python

**Project URL:** 

**Source Location:** https://github.com/lightbulb-framework/lightbulb-framework





**Lynis** 
-----------
**SBB Description:** Lynis is a suite of tools (shell scripts) for security auditing, compliance and hardening for Linux, Mac OS, and Unix based systems. Of course many (better) audit tools are available, but this one is simple and straightforward. So easy to extend and to improve. Especially if you like shell-scripting.
Michael Boelen from the Netherlands (owner of  company cisofy.com ) created this software.
&#160;

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** unix-shell scripts

**Project URL:** https://cisofy.com

**Source Location:** https://github.com/CISOfy/lynis/





**Malspider** 
---------------
**SBB Description:** Malspider is a web spidering framework that detects characteristics of web compromises. 
Based on Scrapy framework?
Malspider is a web spidering framework that inspects websites for characteristics of compromise. Malspider has three purposes:

Website Integrity Monitoring: monitor your organization&#8217;s website (or your personal website) for potentially malicious changes.
Generate Threat Intelligence: keep an eye on previously compromised sites, currently compromised sites, or sites that may be targeted by various threat actors.
Validate Web Compromises: Is this website still compromised?

What can Malspider detect?
Malspider has built-in detection for characteristics of compromise like hidden iframes, reconnaisance frameworks, vbscript injection, email address disclosure, etc.

**SBB License:** BSD License 2.0 (3-clause, New or Revised) License

**Core Technology:** Python

**Project URL:** https://github.com/ciscocsirt/malspider

**Source Location:** https://github.com/ciscocsirt/malspider





**Mantra** 
------------
**SBB Description:** OWASP Mantra is a collection of free and open source tools integrated into a web browser, which can become handy for students, penetration testers, web application developers,security professionals etc. It is portable, ready-to-run, compact and follows the true spirit of free and open source software.
Mantra is lite, flexible, portable and user friendly with a nice graphical user interface. You can carry it in memory cards, flash drives, CD/DVDs, etc. It can be run natively on Linux, Windows and Mac platforms. It can also be installed on to your system within minutes. Mantra is absolutely free of cost and takes no time for you to set up.
Mantra is a browser especially designed for web application security testing. By having such a product, more people will come to know the easiness and flexibility of being able to follow basic testing procedures within the browser. Mantra believes that having such a portable, easy to use and yet powerful platform can be helpful for the industry.
Mantra has many built in tools to modify headers, manipulate input strings, replay GET/POST requests, edit cookies, quickly switch between multiple proxies, control forced redirects etc. This makes it a good software for performing basic security checks and sometimes, exploitation. Thus, Mantra can be used to solve basic levels of various web based CTFs, showcase security issues in vulnerable web applications etc.

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** javascript

**Project URL:** http://www.getmantra.com

**Source Location:** https://code.google.com/p/getmantra/





**Mitmproxy** 
---------------
**SBB Description:** An interactive SSL-capable intercepting HTTP proxy for penetration testers and software developers. Console program that allows traffic flows to be intercepted, inspected, modified and replayed.
Part of mitmproxy is mitmdump is the command-line companion to mitmproxy. It provides tcpdump-like functionality to let you view, record, and programmatically transform HTTP traffic. See the --help flag output for complete documentation.

**SBB License:** MIT License

**Core Technology:** Python

**Project URL:** https://mitmproxy.org

**Source Location:** https://github.com/mitmproxy/mitmproxy





**ModSecurity** 
-----------------
**SBB Description:** ModSecurity is an open source, cross-platform web application firewall (WAF) module. Known as the &#8220;Swiss Army Knife&#8221; of WAFs, it enables web application defenders to gain visibility into HTTP(S) traffic and provides a power rules language and API to implement advanced protections.
ModSecurity is an open source, cross platform web application firewall (WAF) engine for Apache, IIS and Nginx that is developed by Trustwave&#8217;s SpiderLabs. It has a robust event-based programming language which provides protection from a range of attacks against web applications and allows for HTTP traffic monitoring, logging and real-time analyse.

**SBB License:** Apache License 2.0

**Core Technology:** C

**Project URL:** http://www.modsecurity.org/

**Source Location:** https://github.com/SpiderLabs/ModSecurity





**OpenVAS** 
-------------
**SBB Description:** OpenVAS is a framework of several services and tools offering a comprehensive and powerful vulnerability scanning and vulnerability management solution.
The core of this SSL-secured service-oriented architecture is the OpenVAS Scanner. The scanner very efficiently executes the actual Network Vulnerability Tests (NVTs) which are served with daily updates via the OpenVAS NVT Feed or via a commercial feed service.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** http://www.openvas.org

**Source Location:** https://scm.wald.intevation.org/svn/openvas/trunk





**osquery** 
-------------
**SBB Description:** SQL powered operating system instrumentation, monitoring, and analytics. Osquery exposes an operating system as a high-performance relational database. This allows you to write SQL-based queries to explore operating system data. With osquery, SQL tables represent abstract concepts such as running processes, loaded kernel modules, open network connections, browser plugins, hardware events or file hashes.
Developed by Facebook.
&#160;

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** https://osquery.io/

**Source Location:** https://github.com/facebook/osquery





**OWASP ZCR Shellcoder** 
--------------------------
**SBB Description:** OWASP ZCR Shellcoder is an open source software in python language which lets you generate customized shellcodes for various operation systems. Shellcodesare small codes in assembly which could be use as the payload in software exploiting. Other usages are in malwares, bypassing antiviruses, obfuscated codes and etc.
&#160;

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** Python

**Project URL:** https://www.owasp.org/index.php/OWASP_ZSC_Tool_Project

**Source Location:** https://github.com/Ali-Razmjoo/OWASP-ZSC/





**OWASP Zed Attack Proxy (ZAP)** 
----------------------------------
**SBB Description:** The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.
It is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox.

**SBB License:** Apache License 2.0

**Core Technology:** Java

**Project URL:** https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project#tab=Main

**Source Location:** https://github.com/zaproxy/zaproxy





**Phpseclib (PHP Secure Communications Library)** 
---------------------------------------------------
**SBB Description:** Phpseclib is designed to be ultra-compatible. It works on PHP4+ (PHP4, assuming the use of PHP_Compat) and doesn&#8217;t require any extensions. For purposes of speed, mcrypt is used if it&#8217;s available as is gmp or bcmath (in that order), but they are not required. Phpseclib is designed to be fully interoperable with OpenSSL and other standardized cryptography programs and protocols.
Phpseclib is a pure-PHP implementations of:

BigIntegers
RSA
SSH2
SFTP
X.509
Symmetric key encryption


AES
Rijndael
Twofish
Blowfish
DES
3DES
RC4
RC2

**SBB License:** MIT License

**Core Technology:** PHP

**Project URL:** http://phpseclib.sourceforge.net/

**Source Location:** https://github.com/phpseclib/phpseclib





**Radare** 
------------

**SBB Description:** Unix-like reverse engineering framework and commandline tools.

Radare is a portable reversing framework that can:

- Disassemble (and assemble for) many different architectures
- Debug with local native and remote debuggers (gdb, rap, webui, r2pipe, winedbg, windbg)
- Run on Linux, BSD, Windows, OSX, Android, iOS, Solaris and Haiku
- Perform forensics on filesystems and data carving
- Be scripted in Python, Javascript, Go and more
- Support collaborative analysis using the embedded webserver
- Visualize data structures of several file types
- Patch programs to uncover new features or fix vulnerabilities
- Use powerful analysis capabilities to speed up reversing
- Aid in software exploitation

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** C

**Project URL:** http://rada.re/r/index.html

**Source Location:** https://github.com/radare/radare2





**Requests: HTTP for Humans** 
-------------------------------
**SBB Description:** Requests is the only Non-GMO HTTP library for Python, safe for human consumption.
Requests allows you to send organic, grass-fed HTTP/1.1 requests, without the need for manual labor. There&#8217;s no need to manually add query strings to your URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling are 100% automatic, powered by urllib3, which is embedded within Requests.

**SBB License:** Apache License 2.0

**Core Technology:** Python

**Project URL:** 

**Source Location:** https://github.com/kennethreitz/requests





**RIPS (code analyser)** 
--------------------------
**SBB Description:** RIPS is a tool written in PHP to find vulnerabilities in PHP applications using static code analysis. By tokenizing and parsing all source code files RIPS is able to transform PHP source code into a program model and to detect sensitive sinks (potentially vulnerable functions) that can be tainted by userinput (influenced by a malicious user) during the program flow. Besides the structured output of found vulnerabilities RIPS also offers an integrated code audit framework for further manual analysis.
RIPS was released during the Month of PHP Security (www.php-security.org).
Features


detect XSS, SQLi, File disclosure, LFI/RFI, RCE vulnerabilities and more
5 verbosity levels for debugging your scan results
mark vulnerable lines in source code viewer
highlight variables in the code viewer
user-defined function code by mouse-over on detected call
active jumping between function declaration and calls
list of all user-defined functions (defines and calls), program entry points (user input) and scanned files (with includes) connected to the source code viewer
graph visualization for files and includes as well as functions and calls
create CURL exploits for detected vulnerabilities with few clicks
visualization, description, example, PoC, patch and securing function list for every vulnerability
7 different syntax highlighting colour schemata
display scan result in form of a top-down flow or bottom-up trace
only minimal requirement is a local web server with PHP and a browser (tested with Firefox)
regex search function

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** PHP

**Project URL:** http://rips-scanner.sourceforge.net/

**Source Location:** http://sourceforge.net/projects/rips-scanner/





**RouterSploit** 
------------------
**SBB Description:** The RouterSploit Framework is an open-source exploitation framework dedicated to embedded devices.
It consists of various modules that aids penetration testing operations:

exploits &#8211; modules that take advantage of identified vulnerabilities
creds &#8211; modules designed to test credentials against network services
scanners &#8211; modules that check if target is vulnerable to any exploit

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python

**Project URL:** https://github.com/reverse-shell/routersploit

**Source Location:** https://github.com/reverse-shell/routersploit





**Security Monkey** 
---------------------
**SBB Description:** Security Monkey monitors policy changes and alerts on insecure configurations in an AWS account. While Security Monkey’s main purpose is security, it also proves a useful tool for tracking down potential problems as it is essentially a change tracking system.
More information: http://techblog.netflix.com/2014/06/announcing-security-monkey-aws-security.html

**SBB License:** Apache License 2.0

**Core Technology:**  Python

**Project URL:** http://securitymonkey.readthedocs.org/en/latest/

**Source Location:** https://github.com/Netflix/security_monkey





**SIMP (The System Integrity Management Platform)** 
-----------------------------------------------------
**SBB Description:** SIMP is a framework that aims to provide a reasonable combination of security compliance and operational flexibility. Fundamentally, SIMP is a framework that is designed to be secure from a practical point of view out of the box. As a framework, SIMP is designed to be flexed to meet the needs of the end user.
The ultimate goal of the project is to provide a complete management environment focused on compliance with the various profiles in the SCAP Security Guide Project and industry best practice.
Though it is fully capable out of the box, the intent of SIMP is to be molded to your target environment in such a way that deviations are easily identifiable to both Operations Teams and Security Officers. This project is released to the public by the US National Security Agency.

**SBB License:** MIT License

**Core Technology:** 

**Project URL:** https://github.com/NationalSecurityAgency/SIMP

**Source Location:** https://github.com/simp





**Simplify** 
--------------
**SBB Description:** Simplify uses a virtual machine to understand what an app does. Then, it applies optimizations to create code that behaves identically, but is easier for a human to understand. Specifically, it takes Smali files as input and outputs a Dex file with (hopefully) identical semantics but less complicated structure.
For example, if an app&#8217;s strings are encrypted, Simplify will interpret the app in its own virtual machine to determine semantics. Then, it uses the apps own code to decrypt the strings and replaces the encrypted strings and the decryption method calls with the decrypted versions. It&#8217;s a generic deobfuscator because Simplify doesn&#8217;t need to know how the decryption works ahead of time. This technique also works well for eliminating different types of white noise, such as no-ops and useless arithmetic.

**SBB License:** MIT License

**Core Technology:** 

**Project URL:** 

**Source Location:** https://github.com/CalebFenton/simplify





**Streisand** 
---------------
**SBB Description:** Streisand is software for setting up secure connections with your friends. A bit like TOR. Communication can be sets up over  L2TP/IPsec, OpenSSH, OpenVPN, Shadowsocks, sslh, Stunnel, and a Tor bridge.
&#160;
&#160;

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** Python

**Project URL:** https://github.com/jlund/streisand

**Source Location:** https://github.com/jlund/streisand





**Stunnel** 
-------------
**SBB Description:** Stunnel is a proxy designed to add TLS encryption functionality to existing clients and servers without any changes in the programs&#8217; code. Its architecture is optimized for security, portability, and scalability (including load-balancing), making it suitable for large deployments.
Stunnel uses the OpenSSL library for cryptography, so it supports whatever cryptographic algorithms are compiled into the library. It can benefit from the FIPS 140-2 validation of the OpenSSL FIPS Object Module, as long as the building process meets its Security Policy.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** https://www.stunnel.org/index.html

**Source Location:** http://www.usenix.org.uk/mirrors/stunnel/





**Suricata** 
--------------
**SBB Description:** Suricata is a high performance Network IDS, IPS and Network Security Monitoring engine. Open Source and owned by a community run non-profit foundation, the Open Information Security Foundation (OISF). Suricata is developed by the OISF and its supporting vendors.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** C

**Project URL:** http://suricata-ids.org

**Source Location:** https://github.com/inliniac/suricata





**SWAMP (Software Assurance Marketplace)** 
--------------------------------------------
**SBB Description:** This security application is a SAAS solution. However it is built of OSS building blocks and available to be use under an friendly OSS license for everyone.

Capabilities of the SWAMP
Static analysis
Operates on the original source code
Tracks problems down to the location in the original code
Relatively quick and easy to use
Provides complete code coverage
Compare results from multiple tools
Find and visualize overlaps
Correlate results

Languages supported: C/C++,Java source, Java bytecode, Python, Ruby.  PHP and Javascript are on the roadmap for end 2015 to be supported.

**SBB License:** GNU General Public License (GPL) 3.0

**Core Technology:** 

**Project URL:** https://www.mir-swamp.org

**Source Location:** 





**Tamper Chrome** 
-------------------
**SBB Description:** Tamper Chrome is a Chrome extension that allows you to modify HTTP requests on the fly and aid on web security testing. Tamper Chrome works across all operating systems (including Chrome OS).

**SBB License:** Apache License 2.0

**Core Technology:** Javascript

**Project URL:** https://github.com/google/tamperchrome

**Source Location:** https://github.com/google/tamperchrome





**Threat Dragon** 
-------------------
**SBB Description:** Threat Dragon is a free, open-source threat modelling tool from OWASP.
Threat Dragon is an online threat modelling web application including system diagramming and a rule engine to auto-generate threats/mitigations. The focus will be on great UX a powerful rule engine and alignment with other development lifecycle tools.
ThreatDragon is a Single Page Application (SPA) using Angular on the client and node.js on the server.
Thread Dragon is currently in alfa stage.

**SBB License:** MIT License

**Core Technology:** Javascript / NodeJS

**Project URL:** https://www.owasp.org/index.php/OWASP_Threat_Dragon

**Source Location:** https://github.com/mike-goodwin/owasp-threat-dragon





**Tlsfuzzer** 
---------------
**SBB Description:** TLS test suite and fuzze. Fuzzer and test suite for TLS (v1.0, v1.1, v1.2) implementations.

tlsfuzzer verifies only TLS level behaviour, it does not perform any checks on the certificate (like hostname validation, CA signatures or key usage). It does however verify if the signatures made on TLS message by the server (like in Server Key Exchange message) match the certificate sent by the server.

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Python

**Project URL:** https://github.com/tomato42/tlsfuzzer

**Source Location:** https://github.com/tomato42/tlsfuzzer





**Tor** 
---------
**SBB Description:** Tor is free software and an open network that helps you defend against traffic analysis, a form of network surveillance that threatens personal freedom and privacy, confidential business activities and relationships, and state security. Creating your own Tor network is easy with this software, or use existing Tor nodes.
&#160;

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** 

**Project URL:** https://www.torproject.org

**Source Location:** https://www.torproject.org/dist/





**Vault** 
-----------
**SBB Description:** Vault is a tool for securely accessing secrets. A secret is anything that you want to tightly control access to, such as API keys, passwords, certificates, and more. Vault provides a unified interface to any secret, while providing tight access control and recording a detailed audit log.
Vault secures, stores, and tightly controls access to tokens, passwords, certificates, API keys, and other secrets in modern computing. Vault handles leasing, key revocation, key rolling, and auditing. Vault presents a unified API to access multiple backends: HSMs, AWS IAM, SQL databases, raw key/value, and more.
A modern system requires access to a multitude of secrets: database credentials, API keys for external services, credentials for service-oriented architecture communication, etc. Understanding who is accessing what secrets is already very difficult and platform-specific. Adding on key rolling, secure storage, and detailed audit logs is almost impossible without a custom solution. This is where Vault steps in.

**SBB License:** Mozilla Public License (MPL) 1.1

**Core Technology:** GO

**Project URL:** https://vaultproject.io

**Source Location:** https://github.com/hashicorp/vault





**VSAQ: Vendor Security Assessment Questionnaire** 
----------------------------------------------------
**SBB Description:** VSAQ is an interactive questionnaire application. Its initial purpose was to support security reviews by facilitating not only the collection of information, but also the redisplay of collected data in templated form.
At Google, questionnaires like the ones in this repository are used to assess the security programs of third parties. But the templates provided can be used for a variety of purposes, including doing a self-assessment of your own security program, or simply becoming familiar with issues affecting the security of web applications.

**SBB License:** Apache License 2.0

**Core Technology:** Javascript

**Project URL:** https://vsaq-demo.withgoogle.com/

**Source Location:** https://github.com/google/vsaq





**w3af (Web Application Attack and Audit Framework)** 
-------------------------------------------------------
**SBB Description:** w3af is a Web Application Attack and Audit Framework. The project’s goal is to create a framework to help you secure your web applications by finding and exploiting all web application vulnerabilities.
The w3af framework is divided into three main sections:

The core, which coordinates the whole process and provides libraries for using in plugins.
The user interfaces, which allow the user to configure and start scans
The plugins, which find links and vulnerabilities

**SBB License:** GNU General Public License (GPL) 2.0

**Core Technology:** Phython

**Project URL:** http://w3af.org/

**Source Location:** https://github.com/andresriancho/w3af/





**YARA** 
----------
**SBB Description:** ARA is a tool aimed at (but not limited to) helping malware researchers to identify and classify malware samples. With YARA you can create descriptions of malware families (or whatever you want to describe) based on textual or binary patterns.

**SBB License:** MIT License

**Core Technology:** C

**Project URL:** https://virustotal.github.io/yara/

**Source Location:** https://github.com/virustotal/yara





End of SBB list <br>
