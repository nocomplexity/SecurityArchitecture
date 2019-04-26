AIL framework
-------------

AIL is a modular framework to analyse potential information leaks from
unstructured data sources like pastes from Pastebin or similar services
or unstructured data streams. AIL framework is flexible and can be
extended to support other functionalities to mine or process sensitive
information (e.g. data leak prevention).

Many features are provided within this framework. E.g.:

-  Modular architecture to handle streams of unstructured or structured
   information.
-  Default support for external ZMQ feeds, such as provided by CIRCL or
   other providers.
-  Multiple feed support: Each module can process and reprocess the
   information already processed by AIL.
-  Detecting and extracting URLs including their geographical location
   (e.g. IP address location).
-  Extracting and validating potential leak of credit cards numbers,
   credentials, …
-  Extracting and validating email addresses leaked including DNS MX
   validation.
-  Module for extracting Tor .onion addresses (to be further processed
   for analysis).
-  Keep tracks of duplicates (and diffing between each duplicate found)
   Extracting and validating potential hostnames (e.g. to feed Passive
   DNS systems).
-  A full-text indexer module to index unstructured information
   Statistics on modules and web.

+-----------------------+-----------------------------------------------+
| **SBB License**       | GNU Affero General Public License Version 3   |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | Python                                        |
+-----------------------+-----------------------------------------------+
| **Project URL**       | https://github.com/CIRCL/AIL-framework        |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/CIRCL/AIL-framework        |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Python, Security                              |
+-----------------------+-----------------------------------------------+

| 

American fuzzy lop
------------------

*American fuzzy lop* is a security-oriented
`fuzzer <https://en.wikipedia.org/wiki/Fuzz_testing>`__ that employs a
novel type of compile-time instrumentation and genetic algorithms to
automatically discover clean, interesting test cases that trigger new
internal states in the targeted binary. This substantially improves the
functional coverage for the fuzzed code.

These tool can be very productive in determining security flaws: The
famous SSL Heartbleed bug was found in record time using this software.
See
https://blog.hboeck.de/archives/868-How-Heartbleed-couldve-been-found.html.

+-----------------------+--------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0       |
+-----------------------+--------------------------------------------+
| **Core Technology**   | C                                          |
+-----------------------+--------------------------------------------+
| **Project URL**       | http://lcamtuf.coredump.cx/afl/            |
+-----------------------+--------------------------------------------+
| **Source Location**   | http://lcamtuf.coredump.cx/afl/releases/   |
+-----------------------+--------------------------------------------+
| **Tag(s)**            | Security, Test Tool                        |
+-----------------------+--------------------------------------------+

| 

Bandit
------

Bandit is a tool designed to find common security issues in Python code.
To do this Bandit processes each file, builds an AST from it, and runs
appropriate plugins against the AST nodes. Once Bandit has finished
scanning all the files it generates a report.

Bandit was originally developed within the OpenStack Security Project
and later rehomed to PyCQA.

+-----------------------+------------------------------------+
| **SBB License**       | Apache License 2.0                 |
+-----------------------+------------------------------------+
| **Core Technology**   | Python                             |
+-----------------------+------------------------------------+
| **Project URL**       | https://github.com/PyCQA/bandit    |
+-----------------------+------------------------------------+
| **Source Location**   | https://github.com/PyCQA/bandit    |
+-----------------------+------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning   |
+-----------------------+------------------------------------+

| 

Bosun
-----

Bosun is an open-source, MIT licensed, monitoring and alerting system by
Stack Exchange. It has an expressive domain specific language for
evaluating alerts and creating detailed notifications. It also lets you
test your alerts against history for a faster development experience.

Collecting metrics about our systems is fun but what makes a monitoring
system useful is alerting when anomalies arise. This is the real
strength of Bosun.

Bosun encourages a particular workflow that makes it easy to design,
test, and deploy an alert. If you look at the top of the Bosun display,
the tabs include Items, Graph, Expression, Rule, and Test config in
left-to-right order; that reflects the phases you go through as you
create an alert. In general, first you’ll select an item (metric) that
is the basis of the alert.

+-----------------------+------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0     |
+-----------------------+------------------------------------------+
| **Core Technology**   | GO                                       |
+-----------------------+------------------------------------------+
| **Project URL**       | http://bosun.org/                        |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/bosun-monitor/bosun   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | Security, SIEM                           |
+-----------------------+------------------------------------------+

| 

Cameradar
---------

Cameradar hacks its way into RTSP videosurveillance cameras.

Cameradar allows you to

-  **Detect open RTSP hosts** on any accessible target host
-  Detect which device model is streaming
-  Launch automated dictionary attacks to get their **stream route**
   (e.g.: ``/live.sdp``)
-  Launch automated dictionary attacks to get the **username and
   password** of the cameras
-  Retrieve a complete and user-friendly report of the results

+-----------------------+-----------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0          |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | GOlang                                        |
+-----------------------+-----------------------------------------------+
| **Project URL**       | https://github.com/Ullaakut/cameradar         |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/Ullaakut/cameradar         |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Security, Test Tool, Vulnerability scanning   |
+-----------------------+-----------------------------------------------+

| 

CLIP OS
-------

The CLIP OS project is an open source project maintained by the `ANSSI
(National Cybersecurity Agency of France) <https://ssi.gouv.fr/en>`__
that aims to build a secure, multi-level operating system, based on the
Linux kernel and a lot of free and open source software.

Documentation can be found on: https://docs.clip-os.org/index.html

+-----------------------+------------------------------------------------+
| **SBB License**       | GNU Lesser General Public License (LGPL) 3.0   |
+-----------------------+------------------------------------------------+
| **Core Technology**   | C                                              |
+-----------------------+------------------------------------------------+
| **Project URL**       | https://clip-os.org/en/                        |
+-----------------------+------------------------------------------------+
| **Source Location**   | https://github.com/CLIPOS/                     |
+-----------------------+------------------------------------------------+
| **Tag(s)**            | Operating System, Security                     |
+-----------------------+------------------------------------------------+

| 

ClusterFuzz
-----------

ClusterFuzz is a scalable fuzzing infrastructure which finds security
and stability issues in software.

It is used by Google for fuzzing the Chrome Browser, and serves as the
fuzzing backend for `OSS-Fuzz <https://github.com/google/oss-fuzz>`__.

ClusterFuzz provides many features which help seamlessly integrate
fuzzing into a software project’s development process:

-  Highly scalable. Google’s internal instance runs on over 25,000
   machines.
-  Accurate deduplication of crashes.
-  Fully automatic bug filing and closing for issue trackers
   (`Monorail <https://opensource.google.com/projects/monorail>`__ only
   for now).
-  Testcase minimization.
-  Regression finding through
   `bisection <https://en.wikipedia.org/wiki/Bisection_(software_engineering)>`__.
-  Statistics for analyzing fuzzer performance, and crash rates.
-  Easy to use web interface for management and viewing crashes.
-  Support for coverage guided fuzzing (e.g. libFuzzer and AFL) and
   blackbox fuzzing.

ClusterFuzz is written in Python and Go

+-----------------------+-----------------------------------------+
| **SBB License**       | Apache License 2.0                      |
+-----------------------+-----------------------------------------+
| **Core Technology**   | Python, GO                              |
+-----------------------+-----------------------------------------+
| **Project URL**       | https://github.com/google/clusterfuzz   |
+-----------------------+-----------------------------------------+
| **Source Location**   | https://github.com/google/clusterfuzz   |
+-----------------------+-----------------------------------------+
| **Tag(s)**            | Python, Security                        |
+-----------------------+-----------------------------------------+

| 

Data Seal
---------

Data Seal is a lightweight, UELMA-compliant data authentication service.

Data Seal is a project of `U.S. Open Data <http://usopendata.org/>`__ to
provide a system where open data released by governments can be
authenticated by end users—whether or not the data was most recently
downloaded from the official source.

Government data releases need to abide by local laws (for example, the
District of Columbia Official Code) and should also abide by the
`Uniform Electronic Legal Material Act
(UELMA) <https://github.com/unitedstates/data-seal/wiki/UELMA>`__. Part
of the UELMA provisions state that “legal material be…authenticated, by
providing a method to determine that it is unaltered”.

Data Seal provides agencies with a web-based interface to provide this
functionality.

+-----------------------+--------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0             |
+-----------------------+--------------------------------------------------+
| **Core Technology**   | Django/Python                                    |
+-----------------------+--------------------------------------------------+
| **Project URL**       | https://github.com/unitedstates/data-seal/wiki   |
+-----------------------+--------------------------------------------------+
| **Source Location**   | https://github.com/unitedstates/data-seal        |
+-----------------------+--------------------------------------------------+
| **Tag(s)**            | data authentication, Security                    |
+-----------------------+--------------------------------------------------+

| 

Datastream
----------

An open-source framework for real-time anomaly detection using Python,
ElasticSearch and Kiban. Also uses scikit-learn.

+-----------------------+------------------------------------------------------+
| **SBB License**       | Apache License 2.0                                   |
+-----------------------+------------------------------------------------------+
| **Core Technology**   | Python                                               |
+-----------------------+------------------------------------------------------+
| **Project URL**       | https://github.com/MentatInnovations/datastream.io   |
+-----------------------+------------------------------------------------------+
| **Source Location**   | https://github.com/MentatInnovations/datastream.io   |
+-----------------------+------------------------------------------------------+
| **Tag(s)**            | ML, Monitoring, Security                             |
+-----------------------+------------------------------------------------------+

| 

Deeptracy
---------

Deeptracy scans your project dependencies to spot vulnerabilities. Is a
meta tool to analyze the security issues in third party libraries used
in your project.

+-----------------------+-----------------------------------------------+
| **SBB License**       | Apache License 2.0                            |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | Python                                        |
+-----------------------+-----------------------------------------------+
| **Project URL**       | https://deeptracy.readthedocs.io/en/latest/   |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/BBVA/deeptracy             |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Security                                      |
+-----------------------+-----------------------------------------------+

| 

Diffoscope
----------

| Diffoscope will try to get to the bottom of what makes files or
  directories different. It will recursively unpack archives of many
  kinds and transform various binary formats into more human readable
  form to compare them. It can compare two tarballs, ISO images, or PDF
  just as easily.
| It can be scripted through error codes, and a report can be produced
  with the detected differences. The report can be text or HTML. When no
  type of report has been selected, diffoscope defaults to write a text
  report on the standard output.

| Diffoscope was initially started by the “reproducible builds” Debian
  project and now being developed as part of the (wider) “Reproducible
  Builds” initiative. It is meant
| to be able to quickly understand why two builds of the same package
  produce different outputs. diffoscope was previously named debbindiff.

+-----------------------+-----------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0                      |
+-----------------------+-----------------------------------------------------------+
| **Core Technology**   | Python, CPP                                               |
+-----------------------+-----------------------------------------------------------+
| **Project URL**       | https://diffoscope.org/                                   |
+-----------------------+-----------------------------------------------------------+
| **Source Location**   | https://salsa.debian.org/reproducible-builds/diffoscope   |
+-----------------------+-----------------------------------------------------------+
| **Tag(s)**            | Security                                                  |
+-----------------------+-----------------------------------------------------------+

| 

Duplicity
---------

Duplicity backs directories by producing encrypted tar-format volumes
and uploading them to a remote or local file server.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | http://duplicity.nongnu.org/           |
+-----------------------+----------------------------------------+
| **Source Location**   | https://code.launchpad.net/duplicity   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | backup, Security                       |
+-----------------------+----------------------------------------+

| 

Evilginx2
---------

Standalone man-in-the-middle attack framework used for phishing login
credentials along with session cookies, allowing for the bypass of
2-factor authentication.

This tool is a successor to
`Evilginx <https://github.com/kgretzky/evilginx>`__, released in 2017,
which used a custom version of nginx HTTP server to provide
man-in-the-middle functionality to act as a proxy between a browser and
phished website. Present version is fully written in GO as a standalone
application, which implements its own HTTP and DNS server, making it
extremely easy to set up and use.

+-----------------------+-----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0    |
+-----------------------+-----------------------------------------+
| **Core Technology**   | GO                                      |
+-----------------------+-----------------------------------------+
| **Project URL**       | https://github.com/kgretzky/evilginx2   |
+-----------------------+-----------------------------------------+
| **Source Location**   | https://github.com/kgretzky/evilginx2   |
+-----------------------+-----------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning        |
+-----------------------+-----------------------------------------+

| 

Fail2ban
--------

***Fail2ban*** scans log files (e.g. ``/var/log/apache/error_log``) and
bans IPs that show the malicious signs — too many password failures,
seeking for exploits, etc. Generally Fail2Ban is then used to update
firewall rules to reject the IP addresses for a specified amount of
time, although any arbitrary other **action** (e.g. sending an email)
could also be configured. Out of the box Fail2Ban comes with **filters**
for various services (apache, courier, ssh, etc).

+-----------------------+-----------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0                |
+-----------------------+-----------------------------------------------------+
| **Core Technology**   | Python                                              |
+-----------------------+-----------------------------------------------------+
| **Project URL**       | https://www.fail2ban.org/wiki/index.php/Main_Page   |
+-----------------------+-----------------------------------------------------+
| **Source Location**   | https://github.com/fail2ban                         |
+-----------------------+-----------------------------------------------------+
| **Tag(s)**            | Network, network diagnostic, Python, Security       |
+-----------------------+-----------------------------------------------------+

| 

FIDO (Fully Integrated Defense Operation)
-----------------------------------------

FIDO (Fully Integrated Defense Operation – apologies to the FIDO
Alliance for acronym collision) is developed by NetFlix and is now OSS.
This system is for automatically analyzing security events and
responding to security incidents.

The premise of FIDO is simple… each year companies are receiving an ever
increasing amount of security related alerts. Instead of hiring more
analyst to comb through the endless stream of alerts we automate the
analysis to combat the barrage of information. Simply put, we integrate
and then automate the manual human processes by codifying the logic and
process used by threat analysts to provide consistent and reliable
results.

The typical process for investigating security-related alerts is labor
intensive and largely manual. To make the situation more difficult, as
attacks increase in number and diversity, there is an increasing array
of detection systems deployed and generating even more alerts for
security teams to investigate.

FIDO is a NetFlix OSS project, see:
http://techblog.netflix.com/2015/05/introducing-fido-automated-security.html

+-----------------------+----------------------------------------+
| **SBB License**       | Apache License 2.0                     |
+-----------------------+----------------------------------------+
| **Core Technology**   | C#                                     |
+-----------------------+----------------------------------------+
| **Project URL**       | https://github.com/Netflix/Fido/wiki   |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/Netflix/Fido        |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security, SIEM                         |
+-----------------------+----------------------------------------+

| 

FourOneOne
----------

411 is An Alert Management Web Application. If offers:

-  A Search scheduler.Configure Searches to periodically run against a
   variety of data sources. You can define a custom pipeline of Filters
   to manipulate any generated Alerts and forward them to multiple
   Targets.
-  An alert management interface.Review and manage Alerts through the
   web interface. You can apply renderers to alerts to enrich them with
   additional metadata.

Typical Use cases for 411:

-  You want to detect when certain log lines show up in ES.
-  You want to detect when a Graphite metric changes.
-  You want to detect when a server stops responding
-  You want to manage alerts through a simple workflow. And much more!

A working demo is available at https://demo.fouroneone.io/

+-----------------------+----------------------------------+
| **SBB License**       | MIT License                      |
+-----------------------+----------------------------------+
| **Core Technology**   | PHP                              |
+-----------------------+----------------------------------+
| **Project URL**       | ` <>`__                          |
+-----------------------+----------------------------------+
| **Source Location**   | https://github.com/etsy/411      |
+-----------------------+----------------------------------+
| **Tag(s)**            | Alerting, Loganalyze, Security   |
+-----------------------+----------------------------------+

| 

Ghidra
------

Ghidra is a software reverse engineering (SRE) framework created and
maintained by the `National Security Agency <https://www.nsa.gov>`__
Research Directorate. This framework includes a suite of full-featured,
high-end software analysis tools that enable users to analyze compiled
code on a variety of platforms including Windows, macOS, and Linux.
Capabilities include disassembly, assembly, decompilation, graphing, and
scripting, along with hundreds of other features. Ghidra supports a wide
variety of processor instruction sets and executable formats and can be
run in both user-interactive and automated modes. Users may also develop
their own Ghidra plug-in components and/or scripts using Java or Python.

+-----------------------+----------------------------------------------------+
| **SBB License**       | Apache License 2.0                                 |
+-----------------------+----------------------------------------------------+
| **Core Technology**   | Java                                               |
+-----------------------+----------------------------------------------------+
| **Project URL**       | https://ghidra-sre.org/                            |
+-----------------------+----------------------------------------------------+
| **Source Location**   | https://github.com/NationalSecurityAgency/ghidra   |
+-----------------------+----------------------------------------------------+
| **Tag(s)**            | Security, Test Tool                                |
+-----------------------+----------------------------------------------------+

| 

GNUnet
------

GNUnet is a mesh routing layer for end-to-end encrypted networking and a
framework for distributed applications designed to replace the old
insecure Internet protocol stack.

In other words, GNUnet provides a strong foundation of free software for
a global, distributed network that provides security and privacy. Along
with an application for secure publication of files, it has grown to
include all kinds of basic applications for the foundation of a GNU
internet.

GNUnet is an official GNU package.

The foremost goal of the GNUnet project is to become a widely used,
reliable, open, non-discriminating, egalitarian, unfettered and
censorship-resistant system of free information exchange. We value free
speech above state secrets, law-enforcement or intellectual property.
GNUnet is supposed to be an anarchistic network, where the only
limitation for peers is that they must contribute enough back to the
network such that their resource consumption does not have a significant
impact on other users. GNUnet should be more than just another
file-sharing network. The plan is to offer many other services and in
particular to serve as a development platform for the next generation of
decentralized Internet protocols.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C                                      |
+-----------------------+----------------------------------------+
| **Project URL**       | https://gnunet.org/                    |
+-----------------------+----------------------------------------+
| **Source Location**   | https://gnunet.org/svn/                |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Privacy, Security                      |
+-----------------------+----------------------------------------+

| 

Gophish
-------

Gophish is a powerful, open-source phishing framework that makes it easy
to test your organization’s exposure to phishing.

+-----------------------+--------------------------------------+
| **SBB License**       | MIT License                          |
+-----------------------+--------------------------------------+
| **Core Technology**   | GO                                   |
+-----------------------+--------------------------------------+
| **Project URL**       | https://getgophish.com/              |
+-----------------------+--------------------------------------+
| **Source Location**   | https://github.com/gophish/gophish   |
+-----------------------+--------------------------------------+
| **Tag(s)**            | Security                             |
+-----------------------+--------------------------------------+

| 

Gryffin
-------

Gryffin is a large scale web security scanning platform. Created by
Yahoo, and since September 2015 available as open source.

It is not yet another scanner. It was written to solve two specific
problems with existing scanners: coverage and scale. Better coverage
translates to fewer false negatives. Inherent scalability translates to
capability of scanning, and supporting a large elastic application
infrastructure. Simply put, the ability to scan 1000 applications today
to 100,000 applications tomorrow by straightforward horizontal scaling.

+-----------------------+-----------------------------------------+
| **SBB License**       | MIT License                             |
+-----------------------+-----------------------------------------+
| **Core Technology**   | Go                                      |
+-----------------------+-----------------------------------------+
| **Project URL**       | https://github.com/yahoo/gryffin        |
+-----------------------+-----------------------------------------+
| **Source Location**   | https://github.com/yahoo/gryffin        |
+-----------------------+-----------------------------------------+
| **Tag(s)**            | IDS, Security, Vulnerability scanning   |
+-----------------------+-----------------------------------------+

| 

Hammertime
----------

**Hammertime**: a software suite for testing, profiling and simulating
the rowhammer DRAM defect.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python / C                             |
+-----------------------+----------------------------------------+
| **Project URL**       | https://github.com/vusec/hammertime    |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/vusec/hammertime    |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security, Test Tool                    |
+-----------------------+----------------------------------------+

| 

Hashcat
-------

Hashcat is the world’s fastest and most advanced password recovery
utility, supporting five unique modes of attack for over 200
highly-optimized hashing algorithms. hashcat currently supports CPUs,
GPUs, and other hardware accelerators on Linux, Windows, and macOS, and
has facilities to help enable distributed password cracking.

+-----------------------+--------------------------------------+
| **SBB License**       | MIT License                          |
+-----------------------+--------------------------------------+
| **Core Technology**   | C                                    |
+-----------------------+--------------------------------------+
| **Project URL**       | https://hashcat.net/hashcat/         |
+-----------------------+--------------------------------------+
| **Source Location**   | https://github.com/hashcat/hashcat   |
+-----------------------+--------------------------------------+
| **Tag(s)**            | Password, Security                   |
+-----------------------+--------------------------------------+

| 

Httpswatch
----------

Test tool and site to verify if HTTPS is used as should be for website.

 

+-----------------------+-------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0      |
+-----------------------+-------------------------------------------+
| **Core Technology**   | Python                                    |
+-----------------------+-------------------------------------------+
| **Project URL**       | https://httpswatch.com                    |
+-----------------------+-------------------------------------------+
| **Source Location**   | https://github.com/benjaminp/httpswatch   |
+-----------------------+-------------------------------------------+
| **Tag(s)**            | Security, Test Tool                       |
+-----------------------+-------------------------------------------+

| 

Kali
----

Kali is the most complete ‘Penetration Testing Linux Distribution’
around. Everything you need for penetration testing is collected, tested
and made available on this linux distribution. Of course all tools are
OSS.

The complete list of tools can be found
here:\ http://tools.kali.org/tools-listing

+-----------------------+---------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0        |
+-----------------------+---------------------------------------------+
| **Core Technology**   | N.A. (OSS Tool collection)                  |
+-----------------------+---------------------------------------------+
| **Project URL**       | https://www.kali.org/                       |
+-----------------------+---------------------------------------------+
| **Source Location**   | http://git.kali.org/gitweb/                 |
+-----------------------+---------------------------------------------+
| **Tag(s)**            | Security, Sniffer, Vulnerability scanning   |
+-----------------------+---------------------------------------------+

| 

Keycloak
--------

Keycloak is an Open Source Identity and Access Management solution for
modern Applications and Services.

Users authenticate with Keycloak rather than individual applications.
This means that your applications don’t have to deal with login forms,
authenticating users, and storing users. Once logged-in to Keycloak,
users don’t have to login again to access a different application.

+-----------------------+----------------------------------------+
| **SBB License**       | Apache License 2.0                     |
+-----------------------+----------------------------------------+
| **Core Technology**   | Java                                   |
+-----------------------+----------------------------------------+
| **Project URL**       | https://www.keycloak.org/              |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/keycloak/keycloak   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security                               |
+-----------------------+----------------------------------------+

| 

Kismet
------

Kismet is an 802.11 layer2 wireless network detector, sniffer, and
intrusion detection system. Kismet will work with any wireless card
which supports raw monitoring (rfmon) mode, and (with appropriate
hardware) can sniff 802.11b, 802.11a, 802.11g, and 802.11n traffic.
Kismet also supports plugins which allow sniffing other media such as
DECT.

Kismet identifies networks by passively collecting packets and detecting
standard named networks, detecting (and given time, decloaking) hidden
networks, and inferring the presence of non beaconing networks via data
traffic. The great feature of Kismet is that this tool works working
passively, so detection by IDS is prevented when scanning WLAN’s.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C++                                    |
+-----------------------+----------------------------------------+
| **Project URL**       | http://www.kismetwireless.net/         |
+-----------------------+----------------------------------------+
| **Source Location**   | https://www.kismetwireless.net/code/   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | IDS, Security, Sniffer                 |
+-----------------------+----------------------------------------+

| 

Lascar
------

**L**\ edger’s **A**\ dvanced **S**\ ide **C**\ hannel **A**\ nalysis
**R**\ epository

A fast, versatile, and open source python3 library designed to
facilitate Side-Channel Analysis. Lascar provides primitives for all the
required steps in Side Channel Analysis. It allows the implementaton of
end-to-end Side Channel Attacks.

*lascar* is intended to be used by seasoned side-channel attackers as
well as laymen who would like to get a feel of side-channel analysis.

From side-channel acquisitions to results management, passing by signal
synchronisation, custom attacks, *lascar* provides classes/functions to
solve most of the obstacles an attacker would face, when needed to
perform sound, state-of-the-art side-channel analysis.

+-----------------------+-------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0      |
+-----------------------+-------------------------------------------+
| **Core Technology**   | Python                                    |
+-----------------------+-------------------------------------------+
| **Project URL**       | https://github.com/Ledger-Donjon/lascar   |
+-----------------------+-------------------------------------------+
| **Source Location**   | https://github.com/Ledger-Donjon/lascar   |
+-----------------------+-------------------------------------------+
| **Tag(s)**            | Security                                  |
+-----------------------+-------------------------------------------+

| 

Libreswan
---------

Libreswan is an IPsec implementation for Linux. Libreswan is a free
software implementation of the most widely supported and standarized VPN
protocol based on (“IPsec”) and the Internet Key Exchange (“IKE”).

 

+-----------------------+------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0     |
+-----------------------+------------------------------------------+
| **Core Technology**   |                                          |
+-----------------------+------------------------------------------+
| **Project URL**       | https://libreswan.org/                   |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/libreswan/libreswan   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | communication, Cryptography, Security    |
+-----------------------+------------------------------------------+

| 

Lightbulb
---------

LightBulb is an open source python framework for auditing web
applications firewalls.

Project created and started in 2016.

+-----------------------+--------------------------------------------------------------+
| **SBB License**       | MIT License                                                  |
+-----------------------+--------------------------------------------------------------+
| **Core Technology**   | Python                                                       |
+-----------------------+--------------------------------------------------------------+
| **Project URL**       | ` <>`__                                                      |
+-----------------------+--------------------------------------------------------------+
| **Source Location**   | https://github.com/lightbulb-framework/lightbulb-framework   |
+-----------------------+--------------------------------------------------------------+
| **Tag(s)**            | Audit, Security, Waf                                         |
+-----------------------+--------------------------------------------------------------+

| 

Lynis
-----

Lynis is a suite of tools (shell scripts) for security auditing,
compliance and hardening for Linux, Mac OS, and Unix based systems. Of
course many (better) audit tools are available, but this one is simple
and straightforward. So easy to extend and to improve. Especially if you
like shell-scripting.

Michael Boelen from the Netherlands (owner of  company cisofy.com )
created this software.

 

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | unix-shell scripts                     |
+-----------------------+----------------------------------------+
| **Project URL**       | https://cisofy.com                     |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/CISOfy/lynis/       |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Audit, Security                        |
+-----------------------+----------------------------------------+

| 

Magic Wormhole
--------------

Get things from one computer to another, safely.

This package provides a library and a command-line tool named wormhole,
which makes it possible to get arbitrary-sized files and directories (or
short pieces of text) from one computer to another. The two endpoints
are identified by using identical “wormhole codes”: in general, the
sending machine generates and displays the code, which must then be
typed into the receiving machine.

+-----------------------+----------------------------------------------------+
| **SBB License**       | MIT License                                        |
+-----------------------+----------------------------------------------------+
| **Core Technology**   | Python                                             |
+-----------------------+----------------------------------------------------+
| **Project URL**       | https://magic-wormhole.readthedocs.io/en/latest/   |
+-----------------------+----------------------------------------------------+
| **Source Location**   | https://github.com/warner/magic-wormhole           |
+-----------------------+----------------------------------------------------+
| **Tag(s)**            | Security                                           |
+-----------------------+----------------------------------------------------+

| 

Malspider
---------

Malspider is a web spidering framework that detects characteristics of
web compromises.

Based on Scrapy framework.

Malspider is a web spidering framework that inspects websites for
characteristics of compromise. Malspider has three purposes:

-  **Website Integrity Monitoring**: monitor your organization’s website
   (or your personal website) for potentially malicious changes.
-  **Generate Threat Intelligence:** keep an eye on previously
   compromised sites, currently compromised sites, or sites that may be
   targeted by various threat actors.
-  **Validate Web Compromises**: Is this website still compromised?

Malspider has built-in detection for characteristics of compromise like
hidden iframes, reconnaisance frameworks, vbscript injection, email
address disclosure, etc.

+-----------------------+------------------------------------------------------+
| **SBB License**       | BSD License 2.0 (3-clause, New or Revised) License   |
+-----------------------+------------------------------------------------------+
| **Core Technology**   | Python                                               |
+-----------------------+------------------------------------------------------+
| **Project URL**       | https://github.com/ciscocsirt/malspider              |
+-----------------------+------------------------------------------------------+
| **Source Location**   | https://github.com/ciscocsirt/malspider              |
+-----------------------+------------------------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning                     |
+-----------------------+------------------------------------------------------+

| 

Mantra
------

**OWASP Mantra** is a collection of free and open source tools
integrated into a web browser, which can become handy for students,
penetration testers, web application developers,security professionals
etc. It is portable, ready-to-run, compact and follows the true spirit
of free and open source software.

**Mantra** is lite, flexible, portable and user friendly with a nice
graphical user interface. You can carry it in memory cards, flash
drives, CD/DVDs, etc. It can be run natively on Linux, Windows and Mac
platforms. It can also be installed on to your system within minutes.
Mantra is absolutely free of cost and takes no time for you to set up.

Mantra is a browser especially designed for web application security
testing. By having such a product, more people will come to know the
easiness and flexibility of being able to follow basic testing
procedures within the browser. Mantra believes that having such a
portable, easy to use and yet powerful platform can be helpful for the
industry.

Mantra has many built in tools to modify headers, manipulate input
strings, replay GET/POST requests, edit cookies, quickly switch between
multiple proxies, control forced redirects etc. This makes it a good
software for performing basic security checks and sometimes,
exploitation. Thus, Mantra can be used to solve basic levels of various
web based CTFs, showcase security issues in vulnerable web applications
etc.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | javascript                             |
+-----------------------+----------------------------------------+
| **Project URL**       | http://www.getmantra.com               |
+-----------------------+----------------------------------------+
| **Source Location**   | https://code.google.com/p/getmantra/   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security, Test Tool                    |
+-----------------------+----------------------------------------+

| 

MISP
----

MISP is a threat intelligence platform for gathering, sharing, storing 
and correlating Indicators of Compromise of targeted attacks, threat intelligence, 
financial fraud information, vulnerability information or 
even counter-terrorism information. MISP project is an open source 
threat intelligence platform. The project include utilities and documentation 
for more effective threat intelligence, by sharing indicators of compromise.

Many features are included in this threat intelligence platform. E.g.:

- An efficient IoC and indicators database allowing to store technical  and non-technical information about malware samples, incidents, attackers and intelligence.
- Automatic correlation finding relationships between attributes and indicators from malware, attacks campaigns or analysis.
- Correlation engine includes correlation between attributes and more advanced correlations like Fuzzy hashing correlation (e.g. ssdeep) or CIDR block matching. Correlation can be also enabled or event disabled per attribute.
- A flexible data model where complex objects can be expressed and linked together to express threat intelligence, incidents or connected elements.
- Built-in sharing functionality to ease data sharing using different model of distributions. MISP can synchronize automatically events and attributes among different MISP. Advanced filtering functionalities can be used to meet each organization sharing policy including a flexible sharing group capacity and an attribute level distribution mechanisms.
- An intuitive user-interface for end-users to create, update and collaborate on events and attributes/indicators. A graphical interface to navigate seamlessly between events and their correlations. Advanced filtering functionalities and warning list to help the analysts to contribute events and attributes.
- Storing data in a structured format (allowing automated use of the database for various purposes) with an extensive support of cyber security indicators along fraud indicators as in the financial sector.
- Export: generating IDS (Suricata, Snort and Bro are supported by default), OpenIOC, plain text, CSV, MISP XML or JSON output to integrate with other systems (network IDS, host IDS, custom tools)
- Import: bulk-import, batch-import, free-text import, import from OpenIOC, GFI sandbox, ThreatConnect CSV or MISP format.
- Flexible free text import tool to ease the integration of unstructured reports into MISP.
- A gentle system to collaborate on events and attributes allowing MISP users to propose changes or updates to attributes/indicators.
- data-sharing: automatically exchange and synchronization with other parties and trust-groups using MISP.
- feed import: flexible tool to import and integrate MISP feed and any threatintel or OSINT feed from third parties. Many default feeds are included in standard MISP installation.
- delegating of sharing: allows a simple pseudo-anonymous mechanism to delegate publication of event/indicators to another organization.
- Flexible API to integrate MISP with your own solutions. MISP is bundled with PyMISP which is a flexible Python Library to fetch, add or update events attributes, handle malware samples or search for attributes.
- adjustable taxonomy to classify and tag events following your own classification schemes or existing taxonomies. The taxonomy can be local to your MISP but also shareable among MISP instances. MISP comes with a default set of well-known taxonomies and classification schemes to support standard classification as used by ENISA, Europol, DHS, CSIRTs or many other organisations.
- intelligence vocabularies called MISP galaxy and bundled with existing threat actors, malware, RAT, ransomware or MITRE ATT&CK which can be easily linked with events in MISP.
- expansion modules in Python to expand MISP with your own services or activate already available misp-modules.
- sighting support to get observations from organizations concerning shared indicators and attributes. Sighting can be contributed via MISP user-interface, API as MISP document or STIX sighting documents. Starting with MISP 2.4.66, Sighting has been extended to support false-negative sighting or expiration sighting.
- STIX support: export data in the STIX format (XML and JSON) including export/import in STIX 2.0 format.
- integrated encryption and signing of the notifications via PGP and/or S/MIME depending of the user preferences.


+-----------------------+-----------------------------------------------+
| **SBB License**       | GNU Affero General Public License Version 3   |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | PHP, Python                                   |
+-----------------------+-----------------------------------------------+
| **Project URL**       | https://www.misp-project.org/                 |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/MISP/MISP                  |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Security, Threat Intelligence, TIP            |
+-----------------------+-----------------------------------------------+

| 

MITMEngine
----------

The goal of this project is to allow for accurate detection of HTTPS
interception and robust TLS fingerprinting. This project is based off of
`The Security Impact of HTTPS
Interception <https://zakird.com/papers/https_interception.pdf>`__, and
started as a port to Go of `their processing scripts and
fingerprints <https://github.com/zakird/tlsfingerprints>`__.

In a basic HTTPS connection, a browser (client) establishes a TLS
connection directly to an origin server to send requests and download
content. However, many connections on the Internet are not directly from
a browser to the server serving the website, but instead traverse
through some type of proxy or middlebox (a “monster-in-the-middle” or
MITM). There are many reasons for this behavior, both malicious and
benign.

+-----------------------+------------------------------------------------------------+
| **SBB License**       | BSD License 2.0 (3-clause, New or Revised) License         |
+-----------------------+------------------------------------------------------------+
| **Core Technology**   | GO                                                         |
+-----------------------+------------------------------------------------------------+
| **Project URL**       | https://blog.cloudflare.com/monsters-in-the-middleboxes/   |
+-----------------------+------------------------------------------------------------+
| **Source Location**   | https://github.com/cloudflare/mitmengine                   |
+-----------------------+------------------------------------------------------------+
| **Tag(s)**            | Security, Test Tool                                        |
+-----------------------+------------------------------------------------------------+

| 

Mitmproxy
---------

An interactive SSL-capable intercepting HTTP proxy for penetration
testers and software developers. Console program that allows traffic
flows to be intercepted, inspected, modified and replayed.

Part of mitmproxy is **mitmdump** is the command-line companion to
mitmproxy. It provides tcpdump-like functionality to let you view,
record, and programmatically transform HTTP traffic. See the ``--help``
flag output for complete documentation.

+-----------------------+------------------------------------------+
| **SBB License**       | MIT License                              |
+-----------------------+------------------------------------------+
| **Core Technology**   | Python                                   |
+-----------------------+------------------------------------------+
| **Project URL**       | https://mitmproxy.org                    |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/mitmproxy/mitmproxy   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | HTTP Proxy, Privacy, Security, Sniffer   |
+-----------------------+------------------------------------------+

| 

ModSecurity
-----------

ModSecurity is an open source, cross-platform web application firewall
(WAF) module. Known as the “Swiss Army Knife” of WAFs, it enables web
application defenders to gain visibility into HTTP(S) traffic and
provides a power rules language and API to implement advanced
protections.

ModSecurity is an open source, cross platform web application firewall
(WAF) engine for Apache, IIS and Nginx that is developed by Trustwave’s
SpiderLabs. It has a robust event-based programming language which
provides protection from a range of attacks against web applications and
allows for HTTP traffic monitoring, logging and real-time analyse.

+-----------------------+---------------------------------------------+
| **SBB License**       | Apache License 2.0                          |
+-----------------------+---------------------------------------------+
| **Core Technology**   | C                                           |
+-----------------------+---------------------------------------------+
| **Project URL**       | http://www.modsecurity.org/                 |
+-----------------------+---------------------------------------------+
| **Source Location**   | https://github.com/SpiderLabs/ModSecurity   |
+-----------------------+---------------------------------------------+
| **Tag(s)**            | Security, Waf                               |
+-----------------------+---------------------------------------------+

| 

MOSP
----

A platform to create, edit and share JSON Security objects.

The goal of this platform is to gather security related JSON schemas and
objects. You can use any available schemas in order to create shareable
JSON objects. It also possible to keep an object private even if our
goal is to promote the sharing of information. JSON schemas are always
public.

All content is licensed under CC-BY-SA.

Integration with third-party applications is possible thanks to an API:

-  `JSON Schemas <http://objects.monarc.lu/api/v1/schema>`__
-  `JSON Objects <http://objects.monarc.lu/api/v1/json_object>`__

+-----------------------+-----------------------------------------------+
| **SBB License**       | GNU Affero General Public License Version 3   |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | JSON                                          |
+-----------------------+-----------------------------------------------+
| **Project URL**       | http://objects.monarc.lu/                     |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/CASES-LU/MOSP              |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | JSON, Security                                |
+-----------------------+-----------------------------------------------+

| 

Mozilla HTTP Observatory
------------------------

The Mozilla HTTP Observatory is a set of tools to analyze your website
and inform you if you are utilizing the many available methods to secure
it.

+-----------------------+-----------------------------------------------+
| **SBB License**       | Mozilla Public License (MPL) 1.1              |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | Python                                        |
+-----------------------+-----------------------------------------------+
| **Project URL**       | https://observatory.mozilla.org/              |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/mozilla/http-observatory   |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Python, Security, Vulnerability scanning      |
+-----------------------+-----------------------------------------------+

| 

Mythril
-------

Mythril is a security analysis tool for Ethereum smart contracts. It
uses the `LASER-ethereum symbolic virtual
machine <https://github.com/b-mueller/laser-ethereum>`__ to detect
`various types of
issues <https://github.com/ConsenSys/mythril/blob/master/security_checks.md>`__.
Use it to analyze source code or as a nmap-style black-box blockchain
scanner (an “ethermap” if you will).

 

+-----------------------+----------------------------------------+
| **SBB License**       | MIT License                            |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | https://github.com/ConsenSys/mythril   |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/ConsenSys/mythril   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | BlockChain, Security                   |
+-----------------------+----------------------------------------+

| 

OpenVAS
-------

OpenVAS is a framework of several services and tools offering a
comprehensive and powerful vulnerability scanning and vulnerability
management solution.

The core of this SSL-secured service-oriented architecture is the
**OpenVAS Scanner**. The scanner very efficiently executes the actual
Network Vulnerability Tests (NVTs) which are served with daily updates
via the `OpenVAS NVT
Feed <http://www.openvas.org/openvas-nvt-feed.html>`__ or via a
commercial feed service.

+-----------------------+-------------------------------------------------------------------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0                                                                              |
+-----------------------+-------------------------------------------------------------------------------------------------------------------+
| **Core Technology**   | C                                                                                                                 |
+-----------------------+-------------------------------------------------------------------------------------------------------------------+
| **Project URL**       | http://www.openvas.org                                                                                            |
+-----------------------+-------------------------------------------------------------------------------------------------------------------+
| **Source Location**   | `https://scm.wald.intevation.org/svn/openvas/trunk <%20https://scm.wald.intevation.org/svn/openvas/trunk%20>`__   |
+-----------------------+-------------------------------------------------------------------------------------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning                                                                                  |
+-----------------------+-------------------------------------------------------------------------------------------------------------------+

| 

ORY Hydra
---------

ORY Hydra is a hardened OAuth2 and OpenID Connect server optimized for
low-latency, high throughput, and low resource consumption. ORY Hydra is
not an identity provider (user sign up, user log in, password reset
flow), but connects to your existing identity provider through a consent
app.

+-----------------------+--------------------------------+
| **SBB License**       | Apache License 2.0             |
+-----------------------+--------------------------------+
| **Core Technology**   | GOlang                         |
+-----------------------+--------------------------------+
| **Project URL**       | https://www.ory.sh/            |
+-----------------------+--------------------------------+
| **Source Location**   | https://github.com/ory/hydra   |
+-----------------------+--------------------------------+
| **Tag(s)**            | Security                       |
+-----------------------+--------------------------------+

| 

osquery
-------

SQL powered operating system instrumentation, monitoring, and analytics.
Osquery exposes an operating system as a high-performance relational
database. This allows you to write SQL-based queries to explore
operating system data. With osquery, SQL tables represent abstract
concepts such as running processes, loaded kernel modules, open network
connections, browser plugins, hardware events or file hashes.

Developed by Facebook.

 

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C                                      |
+-----------------------+----------------------------------------+
| **Project URL**       | https://osquery.io/                    |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/facebook/osquery    |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Loganalyze, Monitoring, Security       |
+-----------------------+----------------------------------------+

| 

OWASP ZCR Shellcoder
--------------------

OWASP ZCR Shellcoder is an open source software in python language which
lets you generate customized shellcodes for various operation systems.
Shellcodesare small codes in assembly which could be use as the payload
in software exploiting. Other usages are in malwares, bypassing
antiviruses, obfuscated codes and etc.

 

+-----------------------+----------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0                     |
+-----------------------+----------------------------------------------------------+
| **Core Technology**   | Python                                                   |
+-----------------------+----------------------------------------------------------+
| **Project URL**       | https://www.owasp.org/index.php/OWASP_ZSC_Tool_Project   |
+-----------------------+----------------------------------------------------------+
| **Source Location**   | https://github.com/Ali-Razmjoo/OWASP-ZSC/                |
+-----------------------+----------------------------------------------------------+
| **Tag(s)**            | Security, Test Tool                                      |
+-----------------------+----------------------------------------------------------+

| 

OWASP Zed Attack Proxy (ZAP)
----------------------------

The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated
penetration testing tool for finding vulnerabilities in web
applications.

It is designed to be used by people with a wide range of security
experience and as such is ideal for developers and functional testers
who are new to penetration testing as well as being a useful addition to
an experienced pen testers toolbox.

+-----------------------+---------------------------------------------------------------------------+
| **SBB License**       | Apache License 2.0                                                        |
+-----------------------+---------------------------------------------------------------------------+
| **Core Technology**   | Java                                                                      |
+-----------------------+---------------------------------------------------------------------------+
| **Project URL**       | https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project#tab=Main   |
+-----------------------+---------------------------------------------------------------------------+
| **Source Location**   | https://github.com/zaproxy/zaproxy                                        |
+-----------------------+---------------------------------------------------------------------------+
| **Tag(s)**            | Security                                                                  |
+-----------------------+---------------------------------------------------------------------------+

| 

Phpseclib (PHP Secure Communications Library)
---------------------------------------------

Phpseclib is designed to be ultra-compatible. It works on PHP4+ (PHP4,
assuming the use of
`PHP\_Compat <http://pear.php.net/package/PHP_Compat>`__) and doesn’t
require any extensions. For purposes of speed, **mcrypt is used** if
it’s available **as is gmp or bcmath** (in that order), but they are not
required. Phpseclib is designed to be fully interoperable with OpenSSL
and other standardized cryptography programs and protocols.

Phpseclib is a pure-PHP implementations of:

-  BigIntegers
-  RSA
-  SSH2
-  SFTP
-  X.509
-  Symmetric key encryption

   .. raw:: html

      <div id="ciphers">

   -  AES
   -  Rijndael
   -  Twofish
   -  Blowfish
   -  DES
   -  3DES
   -  RC4
   -  RC2

   .. raw:: html

      </div>

+-----------------------+------------------------------------------+
| **SBB License**       | MIT License                              |
+-----------------------+------------------------------------------+
| **Core Technology**   | PHP                                      |
+-----------------------+------------------------------------------+
| **Project URL**       | http://phpseclib.sourceforge.net/        |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/phpseclib/phpseclib   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | Cryptography, Security                   |
+-----------------------+------------------------------------------+

| 

PySyft
------

| A library for encrypted, privacy preserving deep learning. PySyft is a
  Python library for secure, private Deep Learning. PySyft decouples
  private data from model training, using `Multi-Party Computation
  (MPC) <https://en.wikipedia.org/wiki/Secure_multi-party_computation>`__
  within PyTorch. View the paper on
  `Arxiv <https://arxiv.org/abs/1811.04017>`__.

+-----------------------+---------------------------------------+
| **SBB License**       | Apache License 2.0                    |
+-----------------------+---------------------------------------+
| **Core Technology**   | Python                                |
+-----------------------+---------------------------------------+
| **Project URL**       | https://github.com/OpenMined/PySyft   |
+-----------------------+---------------------------------------+
| **Source Location**   | https://github.com/OpenMined/PySyft   |
+-----------------------+---------------------------------------+
| **Tag(s)**            | Python, Security                      |
+-----------------------+---------------------------------------+

| 

Radare
------

Unix-like reverse engineering framework and commandline tools.

Radare is a portable reversing framework that can:

-  Disassemble (and assemble for) many different architectures
-  Debug with local native and remote debuggers (gdb, rap, webui,
   r2pipe, winedbg, windbg)
-  Run on Linux, \*BSD, Windows, OSX, Android, iOS, Solaris and Haiku
-  Perform forensics on filesystems and data carving
-  Be scripted in Python, Javascript, Go and more
-  Support collaborative analysis using the embedded webserver
-  Visualize data structures of several file types
-  Patch programs to uncover new features or fix vulnerabilities
-  Use powerful analysis capabilities to speed up reversing
-  Aid in software exploitation

+-----------------------+--------------------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0                               |
+-----------------------+--------------------------------------------------------------------+
| **Core Technology**   | C                                                                  |
+-----------------------+--------------------------------------------------------------------+
| **Project URL**       | http://rada.re/r/index.html                                        |
+-----------------------+--------------------------------------------------------------------+
| **Source Location**   | https://github.com/radare/radare2                                  |
+-----------------------+--------------------------------------------------------------------+
| **Tag(s)**            | Debugger, Security, software development, Vulnerability scanning   |
+-----------------------+--------------------------------------------------------------------+

| 

Requests: HTTP for Humans
-------------------------

Requests is the only *Non-GMO* HTTP library for Python, safe for human
consumption.

Requests allows you to send *organic, grass-fed* HTTP/1.1 requests,
without the need for manual labor. There’s no need to manually add query
strings to your URLs, or to form-encode your POST data. Keep-alive and
HTTP connection pooling are 100% automatic, powered by
`urllib3 <https://github.com/shazow/urllib3>`__, which is embedded
within Requests.

+-----------------------+---------------------------------------------+
| **SBB License**       | Apache License 2.0                          |
+-----------------------+---------------------------------------------+
| **Core Technology**   | Python                                      |
+-----------------------+---------------------------------------------+
| **Project URL**       | ` <>`__                                     |
+-----------------------+---------------------------------------------+
| **Source Location**   | https://github.com/kennethreitz/requests    |
+-----------------------+---------------------------------------------+
| **Tag(s)**            | Security, software development, Test Tool   |
+-----------------------+---------------------------------------------+

| 

RIPS (code analyser)
--------------------

RIPS is a tool written in PHP to find vulnerabilities in PHP
applications using static code analysis. By tokenizing and parsing all
source code files RIPS is able to transform PHP source code into a
program model and to detect sensitive sinks (potentially vulnerable
functions) that can be tainted by userinput (influenced by a malicious
user) during the program flow. Besides the structured output of found
vulnerabilities RIPS also offers an integrated code audit framework for
further manual analysis.

RIPS was released during the Month of PHP Security
(`www.php-security.org <http://www.php-security.org>`__).

**Features**

.. raw:: html

   <div class="content editable">

-  detect XSS, SQLi, File disclosure, LFI/RFI, RCE vulnerabilities and
   more
-  5 verbosity levels for debugging your scan results
-  mark vulnerable lines in source code viewer
-  highlight variables in the code viewer
-  user-defined function code by mouse-over on detected call
-  active jumping between function declaration and calls
-  list of all user-defined functions (defines and calls), program entry
   points (user input) and scanned files (with includes) connected to
   the source code viewer
-  graph visualization for files and includes as well as functions and
   calls
-  create CURL exploits for detected vulnerabilities with few clicks
-  visualization, description, example, PoC, patch and securing function
   list for every vulnerability
-  7 different syntax highlighting colour schemata
-  display scan result in form of a top-down flow or bottom-up trace
-  only minimal requirement is a local web server with PHP and a browser
   (tested with Firefox)
-  regex search function

.. raw:: html

   </div>

+-----------------------+-------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0            |
+-----------------------+-------------------------------------------------+
| **Core Technology**   | PHP                                             |
+-----------------------+-------------------------------------------------+
| **Project URL**       | http://rips-scanner.sourceforge.net/            |
+-----------------------+-------------------------------------------------+
| **Source Location**   | http://sourceforge.net/projects/rips-scanner/   |
+-----------------------+-------------------------------------------------+
| **Tag(s)**            | Code Analyzer, Security                         |
+-----------------------+-------------------------------------------------+

| 

RouterSploit
------------

The RouterSploit Framework is an open-source exploitation framework
dedicated to embedded devices.

It consists of various modules that aids penetration testing operations:

-  exploits – modules that take advantage of identified vulnerabilities
-  creds – modules designed to test credentials against network services
-  scanners – modules that check if target is vulnerable to any exploit

+-----------------------+-------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0            |
+-----------------------+-------------------------------------------------+
| **Core Technology**   | Python                                          |
+-----------------------+-------------------------------------------------+
| **Project URL**       | https://github.com/reverse-shell/routersploit   |
+-----------------------+-------------------------------------------------+
| **Source Location**   | https://github.com/reverse-shell/routersploit   |
+-----------------------+-------------------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning                |
+-----------------------+-------------------------------------------------+

| 

SecLists
--------

SecLists is the security tester’s companion. It is a collection of
multiple types of lists used during security assessments. List types
include usernames, passwords, URLs, sensitive data grep strings, fuzzing
payloads, and many more.

This is an OWASP project (incubator) .

+-----------------------+----------------------------------------------------------+
| **SBB License**       | MIT License                                              |
+-----------------------+----------------------------------------------------------+
| **Core Technology**   | n.a.                                                     |
+-----------------------+----------------------------------------------------------+
| **Project URL**       | https://www.owasp.org/index.php/OWASP_SecLists_Project   |
+-----------------------+----------------------------------------------------------+
| **Source Location**   | https://github.com/danielmiessler/SecLists               |
+-----------------------+----------------------------------------------------------+
| **Tag(s)**            | Security, Test Tool                                      |
+-----------------------+----------------------------------------------------------+

| 

Security Monkey
---------------

Security Monkey monitors policy changes and alerts on insecure
configurations in an AWS account. While Security Monkey’s main purpose
is security, it also proves a useful tool for tracking down potential
problems as it is essentially a change tracking system.

More information:
http://techblog.netflix.com/2014/06/announcing-security-monkey-aws-security.html

+-----------------------+----------------------------------------------------+
| **SBB License**       | Apache License 2.0                                 |
+-----------------------+----------------------------------------------------+
| **Core Technology**   | Python                                             |
+-----------------------+----------------------------------------------------+
| **Project URL**       | http://securitymonkey.readthedocs.org/en/latest/   |
+-----------------------+----------------------------------------------------+
| **Source Location**   | https://github.com/Netflix/security_monkey         |
+-----------------------+----------------------------------------------------+
| **Tag(s)**            | Security, SIEM                                     |
+-----------------------+----------------------------------------------------+

| 

SigPloit
--------

SigPloit a signaling security testing framework dedicated to Telecom
Security professionals and reasearchers to pentest and exploit
vulnerabilites in the signaling protocols used in mobile operators
regardless of the geneartion being in use. SigPloit aims to cover all
used protocols used in the operators interconnects SS7, GTP (3G),
Diameter (4G) or even SIP for IMS and VoLTE infrastructures used in the
access layer and SS7 message encapsulation into SIP-T. Recommendations
for each vulnerability will be provided to guide the tester and the
operator the steps that should be done to enhance their security posture

+-----------------------+------------------------------------------+
| **SBB License**       | MIT License                              |
+-----------------------+------------------------------------------+
| **Core Technology**   | Python                                   |
+-----------------------+------------------------------------------+
| **Project URL**       | https://github.com/SigPloiter/SigPloit   |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/SigPloiter/SigPloit   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | pentest, Security                        |
+-----------------------+------------------------------------------+

| 

SIMP (The System Integrity Management Platform)
-----------------------------------------------

SIMP is a framework that aims to provide a reasonable combination of
security compliance and operational flexibility. Fundamentally, SIMP is
a framework that is designed to be secure from a practical point of view
out of the box. As a framework, SIMP is designed to be flexed to meet
the needs of the end user.

The ultimate goal of the project is to provide a complete management
environment focused on compliance with the various profiles in the `SCAP
Security Guide
Project <https://fedorahosted.org/scap-security-guide/>`__ and industry
best practice.

Though it is fully capable out of the box, the intent of SIMP is to be
molded to your target environment in such a way that deviations are
easily identifiable to both Operations Teams and Security Officers. This
project is released to the public by the US National Security Agency.

+-----------------------+--------------------------------------------------+
| **SBB License**       | MIT License                                      |
+-----------------------+--------------------------------------------------+
| **Core Technology**   |                                                  |
+-----------------------+--------------------------------------------------+
| **Project URL**       | https://github.com/NationalSecurityAgency/SIMP   |
+-----------------------+--------------------------------------------------+
| **Source Location**   | https://github.com/simp                          |
+-----------------------+--------------------------------------------------+
| **Tag(s)**            | Audit, Security                                  |
+-----------------------+--------------------------------------------------+

| 

Simplify
--------

Simplify uses a virtual machine to understand what an app does. Then, it
applies optimizations to create code that behaves identically, but is
easier for a human to understand. Specifically, it takes Smali files as
input and outputs a Dex file with (hopefully) identical semantics but
less complicated structure.

For example, if an app’s strings are encrypted, Simplify will interpret
the app in its own virtual machine to determine semantics. Then, it uses
the apps own code to decrypt the strings and replaces the encrypted
strings and the decryption method calls with the decrypted versions.
It’s a **generic** deobfuscator because Simplify doesn’t need to know
how the decryption works ahead of time. This technique also works well
for eliminating different types of white noise, such as no-ops and
useless arithmetic.

+-----------------------+-------------------------------------------+
| **SBB License**       | MIT License                               |
+-----------------------+-------------------------------------------+
| **Core Technology**   |                                           |
+-----------------------+-------------------------------------------+
| **Project URL**       | ` <>`__                                   |
+-----------------------+-------------------------------------------+
| **Source Location**   | https://github.com/CalebFenton/simplify   |
+-----------------------+-------------------------------------------+
| **Tag(s)**            | Code Analyzer, Security                   |
+-----------------------+-------------------------------------------+

| 

Sonarqube
---------

OWASP project. SonarQube provides the capability to not only show health
of an application but also to highlight issues newly introduced. With a
Quality Gate in place, you can fix the leak and therefore improve code
quality systematically.

SonarQube® software (previously called Sonar) is an open source quality
management platform, dedicated to continuously analyze and measure
technical quality, from project portfolio to method. If you wish to
extend the SonarQube platform with open source plugins, have a look at
our plugin library.

+-----------------------+------------------------------------------------+
| **SBB License**       | GNU Lesser General Public License (LGPL) 3.0   |
+-----------------------+------------------------------------------------+
| **Core Technology**   | Java                                           |
+-----------------------+------------------------------------------------+
| **Project URL**       | https://www.sonarqube.org/                     |
+-----------------------+------------------------------------------------+
| **Source Location**   | https://github.com/SonarSource/sonarqube       |
+-----------------------+------------------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning               |
+-----------------------+------------------------------------------------+

| 

SpiderFoot
----------

SpiderFoot is an open source intelligence automation tool. Its goal is
to automate the process of gathering intelligence about a given target,
which may be an IP address, domain name, hostname or network subnet.

SpiderFoot can be used offensively, i.e. as part of a black-box
penetration test to gather information about the target or defensively
to identify what information your organisation is freely providing for
attackers to use against you.

+-----------------------+----------------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0                           |
+-----------------------+----------------------------------------------------------------+
| **Core Technology**   | Python                                                         |
+-----------------------+----------------------------------------------------------------+
| **Project URL**       | https://www.spiderfoot.net/                                    |
+-----------------------+----------------------------------------------------------------+
| **Source Location**   | https://github.com/smicallef/spiderfoot                        |
+-----------------------+----------------------------------------------------------------+
| **Tag(s)**            | pentest, Python, Security, Test Tool, Vulnerability scanning   |
+-----------------------+----------------------------------------------------------------+

| 

Streisand
---------

Streisand is software for setting up secure connections with your
friends. A bit like TOR.

Streisand  is open source software that sets up a communication server
that can run:

-  WireGuard
-   OpenConnect
-   OpenSSH
-   OpenVPN
-   Shadowsocks
-  SSHLH
-   Stunnel,  or a
-  Tor bridge.

After configuration Streisand generates custom instructions to use the
communication service chosen. At the end of the run you are given an
HTML file with instructions that can be shared with friends, family
members, and fellow activists.  Setting up Streisand requires still some
good Unix knowledge for installation and configuration. So it is a bit
of a hassle. (status 2018)

Using Streisand reduces the barrier of entry to running a
VPN/censorship-bypass server for friends and family and makes secure
communication available to more people.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | https://github.com/jlund/streisand     |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/jlund/streisand     |
+-----------------------+----------------------------------------+
| **Tag(s)**            | communication, Privacy, Security       |
+-----------------------+----------------------------------------+

| 

Stunnel
-------

Stunnel is a proxy designed to add TLS encryption functionality to
existing clients and servers without any changes in the programs’ code.
Its architecture is optimized for security, portability, and scalability
(including load-balancing), making it suitable for large deployments.

Stunnel uses the OpenSSL library for cryptography, so it supports
whatever cryptographic algorithms are compiled into the library. It can
benefit from the FIPS 140-2 validation of the OpenSSL FIPS Object
Module, as long as the building process meets its Security Policy.

+-----------------------+---------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0        |
+-----------------------+---------------------------------------------+
| **Core Technology**   | C                                           |
+-----------------------+---------------------------------------------+
| **Project URL**       | https://www.stunnel.org/index.html          |
+-----------------------+---------------------------------------------+
| **Source Location**   | http://www.usenix.org.uk/mirrors/stunnel/   |
+-----------------------+---------------------------------------------+
| **Tag(s)**            | Cryptography, Security                      |
+-----------------------+---------------------------------------------+

| 

Suricata
--------

Suricata is a high performance Network IDS, IPS and Network Security
Monitoring engine. `Open
Source <http://suricata-ids.org/about/open-source/>`__ and owned by a
community run non-profit foundation, the Open Information Security
Foundation (`OISF <http://idsips.wordpress.com/about/oisf/>`__).
Suricata is developed by the OISF and its `supporting
vendors <http://suricata-ids.org/about/consortium/>`__.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C                                      |
+-----------------------+----------------------------------------+
| **Project URL**       | http://suricata-ids.org                |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/inliniac/suricata   |
+-----------------------+----------------------------------------+
| **Tag(s)**            | IDS, Security                          |
+-----------------------+----------------------------------------+

| 

Susanoo
-------

Susanoo is a REST API security testing framework. Features:

-  Configurable inputs/outputs formats
-  API Vulnerability Scan: Normal scanning engine that scans for IDOR,
   Authentication issues, SQL injections, Error stacks.
-  Smoke Scan: Custom output checks for known pocs can be configured to
   run daily.

+-----------------------+-----------------------------------------+
| **SBB License**       | MIT License                             |
+-----------------------+-----------------------------------------+
| **Core Technology**   | Python                                  |
+-----------------------+-----------------------------------------+
| **Project URL**       | https://github.com/ant4g0nist/Susanoo   |
+-----------------------+-----------------------------------------+
| **Source Location**   | https://github.com/ant4g0nist/Susanoo   |
+-----------------------+-----------------------------------------+
| **Tag(s)**            | Security, Test Tool                     |
+-----------------------+-----------------------------------------+

| 

SWAMP (Software Assurance Marketplace)
--------------------------------------

This security application is a SAAS solution. However it is built of OSS
building blocks and available to be use under an friendly OSS license
for everyone.

-  Capabilities of the SWAMP
-  Static analysis
-  Operates on the original source code
-  Tracks problems down to the location in the original code
-  Relatively quick and easy to use
-  Provides complete code coverage
-  Compare results from multiple tools
-  Find and visualize overlaps
-  Correlate results

Languages supported: C/C++,Java source, Java bytecode, Python, Ruby. 
PHP and Javascript are on the roadmap for end 2015 to be supported.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 3.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   |                                        |
+-----------------------+----------------------------------------+
| **Project URL**       | https://www.mir-swamp.org              |
+-----------------------+----------------------------------------+
| **Source Location**   | ` <>`__                                |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Code Analyzer, Security                |
+-----------------------+----------------------------------------+

| 

Tamper Chrome
-------------

Tamper Chrome is a Chrome extension that allows you to modify HTTP
requests on the fly and aid on web security testing. Tamper Chrome works
across all operating systems (including Chrome OS).

+-----------------------+------------------------------------------+
| **SBB License**       | Apache License 2.0                       |
+-----------------------+------------------------------------------+
| **Core Technology**   | Javascript                               |
+-----------------------+------------------------------------------+
| **Project URL**       | https://github.com/google/tamperchrome   |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/google/tamperchrome   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | Audit, Security, Test Tool               |
+-----------------------+------------------------------------------+

| 

Threat Dragon
-------------

Threat Dragon is a free, open-source threat modelling tool from OWASP.

Threat Dragon is an online threat modelling web application including
system diagramming and a rule engine to auto-generate
threats/mitigations. The focus will be on great UX a powerful rule
engine and alignment with other development lifecycle tools.

ThreatDragon is a Single Page Application (SPA) using Angular on the
client and node.js on the server.

Thread Dragon is currently in alfa stage.

+-----------------------+-------------------------------------------------------+
| **SBB License**       | MIT License                                           |
+-----------------------+-------------------------------------------------------+
| **Core Technology**   | Javascript / NodeJS                                   |
+-----------------------+-------------------------------------------------------+
| **Project URL**       | https://www.owasp.org/index.php/OWASP_Threat_Dragon   |
+-----------------------+-------------------------------------------------------+
| **Source Location**   | https://github.com/mike-goodwin/owasp-threat-dragon   |
+-----------------------+-------------------------------------------------------+
| **Tag(s)**            | Modelling, Security                                   |
+-----------------------+-------------------------------------------------------+

| 

Tink
----

Tink provides secure APIs that are easy to use correctly and hard(er) to
misuse. It reduces common crypto pitfalls with user-centered design,
careful implementation and code reviews, and extensive testing. At
Google, Tink is already being used to secure data of many products such
as AdMob, Google Pay, Google Assistant, Firebase, the Android Search
App, etc.

 

+-----------------------+----------------------------------+
| **SBB License**       | Apache License 2.0               |
+-----------------------+----------------------------------+
| **Core Technology**   | Java                             |
+-----------------------+----------------------------------+
| **Project URL**       | https://github.com/google/tink   |
+-----------------------+----------------------------------+
| **Source Location**   | https://github.com/google/tink   |
+-----------------------+----------------------------------+
| **Tag(s)**            | Cryptography, Security           |
+-----------------------+----------------------------------+

| 

Tlsfuzzer
---------

TLS test suite and fuzze. Fuzzer and test suite for TLS (v1.0, v1.1,
v1.2) implementations.

tlsfuzzer verifies only TLS level behaviour, it does not perform any
checks on the certificate (like hostname validation, CA signatures or
key usage). It does however verify if the signatures made on TLS message
by the server (like in Server Key Exchange message) match the
certificate sent by the server.

+-----------------------+-----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0    |
+-----------------------+-----------------------------------------+
| **Core Technology**   | Python                                  |
+-----------------------+-----------------------------------------+
| **Project URL**       | https://github.com/tomato42/tlsfuzzer   |
+-----------------------+-----------------------------------------+
| **Source Location**   | https://github.com/tomato42/tlsfuzzer   |
+-----------------------+-----------------------------------------+
| **Tag(s)**            | Audit, Security, Test Tool              |
+-----------------------+-----------------------------------------+

| 

Tor
---

Tor is free software and an open network that helps you defend against
traffic analysis, a form of network surveillance that threatens personal
freedom and privacy, confidential business activities and relationships,
and state security. Creating your own Tor network is easy with this
software, or use existing Tor nodes.

 

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   |                                        |
+-----------------------+----------------------------------------+
| **Project URL**       | https://www.torproject.org             |
+-----------------------+----------------------------------------+
| **Source Location**   | https://www.torproject.org/dist/       |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Cryptography, Privacy, Security        |
+-----------------------+----------------------------------------+

| 

Unfurl
------

An Entropy-Based Link Vulnerability Analysis Tool.

`unfurl <https://github.com/JLospinoso/unfurl>`__ is a screening tool
for automating URL entropy analysis. The big idea is to find tokens in a
large list of URLs that have low entropy. These might be susceptible to
brute force attacks.

+-----------------------+-------------------------------------------------------------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0                                                            |
+-----------------------+-------------------------------------------------------------------------------------------------+
| **Core Technology**   | Python                                                                                          |
+-----------------------+-------------------------------------------------------------------------------------------------+
| **Project URL**       | https://jlospinoso.github.io/python/unfurl/abrade/hacking/2018/02/08/unfurl-url-analysis.html   |
+-----------------------+-------------------------------------------------------------------------------------------------+
| **Source Location**   | https://github.com/JLospinoso/unfurl                                                            |
+-----------------------+-------------------------------------------------------------------------------------------------+
| **Tag(s)**            | Security                                                                                        |
+-----------------------+-------------------------------------------------------------------------------------------------+

| 

URL Abuse
---------

URL Abuse is a versatile free software for URL review, analysis and
black-list reporting. URL Abuse is composed of a web interface where
requests are submitted asynchronously and a back-end system to process
the URLs into features modules.


Features:

-  HTTP redirects analysis and follows
-  `Google
   Safe-Browsing <https://developers.google.com/safe-browsing/>`__
   lookup
-  `Phishtank <http://www.phishtank.com/api_info.php>`__ lookup
-  `VirusTotal <https://www.virustotal.com/en/documentation/public-api/>`__
   lookup and submission
-  `URL query <https://github.com/CIRCL/urlquery_python_api/>`__ lookup
-  `CIRCL Passive DNS <http://www.circl.lu/services/passive-dns/>`__
   lookup
-  `CIRCL Passive SSL <http://www.circl.lu/services/passive-ssl/>`__
   lookup
-  `Universal WHOIS <https://github.com/Rafiot/uwhoisd>`__ lookup for
   abuse contact
-  Sphinx search interface to RT/RTIR ticketing systems. The
   functionality is disabled by default but can be used to display
   information about existing report of malicious URLs.

Please note that some of the API services will require an API key. The
API keys should be located in the root of the URL Abuse directory. There
is also an online version to use: https://www.circl.lu/urlabuse/

+-----------------------+-----------------------------------------------+
| **SBB License**       | GNU Affero General Public License Version 3   |
+-----------------------+-----------------------------------------------+
| **Core Technology**   | Python                                        |
+-----------------------+-----------------------------------------------+
| **Project URL**       | http://www.circl.lu/services/urlabuse/        |
+-----------------------+-----------------------------------------------+
| **Source Location**   | https://github.com/CIRCL/url-abuse            |
+-----------------------+-----------------------------------------------+
| **Tag(s)**            | Python, Security                              |
+-----------------------+-----------------------------------------------+

| 

Vault
-----

Vault is a tool for securely accessing secrets. A secret is anything
that you want to tightly control access to, such as API keys, passwords,
certificates, and more. Vault provides a unified interface to any
secret, while providing tight access control and recording a detailed
audit log.

Vault secures, stores, and tightly controls access to tokens, passwords,
certificates, API keys, and other secrets in modern computing. Vault
handles leasing, key revocation, key rolling, and auditing. Vault
presents a unified API to access multiple backends: HSMs, AWS IAM, SQL
databases, raw key/value, and more.

A modern system requires access to a multitude of secrets: database
credentials, API keys for external services, credentials for
service-oriented architecture communication, etc. Understanding who is
accessing what secrets is already very difficult and platform-specific.
Adding on key rolling, secure storage, and detailed audit logs is almost
impossible without a custom solution. This is where Vault steps in.

+-----------------------+--------------------------------------+
| **SBB License**       | Mozilla Public License (MPL) 1.1     |
+-----------------------+--------------------------------------+
| **Core Technology**   | GO                                   |
+-----------------------+--------------------------------------+
| **Project URL**       | https://vaultproject.io              |
+-----------------------+--------------------------------------+
| **Source Location**   | https://github.com/hashicorp/vault   |
+-----------------------+--------------------------------------+
| **Tag(s)**            | Security                             |
+-----------------------+--------------------------------------+

| 

VERIS
-----

VERIS The Vocabulary for Event Recording and Incident Sharing.

The Vocabulary for Event Recording and Incident Sharing (VERIS) is a set
of metrics designed to provide a common language for describing security
incidents in a structured and repeatable manner. VERIS is a response to
one of the most critical and persistent challenges in the security
industry – a lack of quality information. VERIS targets this problem by
helping organizations to collect useful incident-related information and
to share that information – anonymously and responsibly – with others.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | http://veriscommunity.net/index.html   |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/vz-risk/veris       |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security                               |
+-----------------------+----------------------------------------+

| 

VSAQ: Vendor Security Assessment Questionnaire
----------------------------------------------

VSAQ is an interactive questionnaire application. Its initial purpose
was to support security reviews by facilitating not only the collection
of information, but also the redisplay of collected data in templated
form.

At Google, questionnaires like the ones in this repository are used to
assess the security programs of third parties. But the templates
provided can be used for a variety of purposes, including doing a
self-assessment of your own security program, or simply becoming
familiar with issues affecting the security of web applications.

+-----------------------+-------------------------------------+
| **SBB License**       | Apache License 2.0                  |
+-----------------------+-------------------------------------+
| **Core Technology**   | Javascript                          |
+-----------------------+-------------------------------------+
| **Project URL**       | https://vsaq-demo.withgoogle.com/   |
+-----------------------+-------------------------------------+
| **Source Location**   | https://github.com/google/vsaq      |
+-----------------------+-------------------------------------+
| **Tag(s)**            | Audit, Questionnaire, Security      |
+-----------------------+-------------------------------------+

| 

w3af (Web Application Attack and Audit Framework)
-------------------------------------------------

w3af is a Web Application Attack and Audit Framework. The project’s goal
is to create a framework to help you secure your web applications by
finding and exploiting all web application vulnerabilities.

The w3af framework is divided into three main sections:

#. The core, which coordinates the whole process and provides libraries
   for using in plugins.
#. The user interfaces, which allow the user to configure and start
   scans
#. The plugins, which find links and vulnerabilities

+-----------------------+------------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0     |
+-----------------------+------------------------------------------+
| **Core Technology**   | Phython                                  |
+-----------------------+------------------------------------------+
| **Project URL**       | http://w3af.org/                         |
+-----------------------+------------------------------------------+
| **Source Location**   | https://github.com/andresriancho/w3af/   |
+-----------------------+------------------------------------------+
| **Tag(s)**            | Audit, Security, Test Tool               |
+-----------------------+------------------------------------------+

| 

Wapiti
------

Wapiti allows you to audit the security of your websites or web
applications.

It performs “black-box” scans (it does not study the source code) of the
web application by crawling the webpages of the deployed webapp, looking
for scripts and forms where it can inject data.

Once it gets the list of URLs, forms and their inputs, Wapiti acts like
a `fuzzer <http://en.wikipedia.org/wiki/Fuzzing>`__, injecting payloads
to see if a script is vulnerable.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | http://wapiti.sourceforge.net/         |
+-----------------------+----------------------------------------+
| **Source Location**   | http://wapiti.sourceforge.net/         |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Security, Vulnerability scanning       |
+-----------------------+----------------------------------------+

| 

Wifite 2
--------

A complete re-write of wifite, a Python script for auditing wireless
networks.

Wifite is an automated wireless attack tool. Wifite was designed for use
with pentesting distributions of Linux, such as Kali Linux, Pentoo,
BackBox; any Linux distributions with wireless drivers patched for
injection. The script appears to also operate with Ubuntu 11/10, Debian
6, and Fedora 16.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | Python                                 |
+-----------------------+----------------------------------------+
| **Project URL**       | https://github.com/derv82/wifite2      |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/derv82/wifite2      |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Audit, pentest, Security               |
+-----------------------+----------------------------------------+

| 

WireGuard
---------

WireGuard is an extremely simple yet fast and modern VPN that utilizes
state-of-the-art cryptography. It aims to be faster, simpler, leaner,
and more useful than IPSec, while avoiding the massive headache. It
intends to be considerably more performant than OpenVPN. WireGuard is
designed as a general purpose VPN for running on embedded interfaces and
super computers alike, fit for many different circumstances. Initially
released for the Linux kernel, it plans to be cross-platform and widely
deployable. It is currently under heavy development, but already it
might be regarded as the most secure, easiest to use, and simplest VPN
solution in the industry.

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C                                      |
+-----------------------+----------------------------------------+
| **Project URL**       | https://www.wireguard.com/             |
+-----------------------+----------------------------------------+
| **Source Location**   | https://git.zx2c4.com/WireGuard/       |
+-----------------------+----------------------------------------+
| **Tag(s)**            | Privacy, Security, VPN                 |
+-----------------------+----------------------------------------+

| 

YARA
----

YARA is a tool aimed at (but not limited to) helping malware researchers
to identify and classify malware samples. With YARA you can create
descriptions of malware families (or whatever you want to describe)
based on textual or binary patterns.

+-----------------------+--------------------------------------+
| **SBB License**       | MIT License                          |
+-----------------------+--------------------------------------+
| **Core Technology**   | C                                    |
+-----------------------+--------------------------------------+
| **Project URL**       | https://virustotal.github.io/yara/   |
+-----------------------+--------------------------------------+
| **Source Location**   | https://github.com/virustotal/yara   |
+-----------------------+--------------------------------------+
| **Tag(s)**            | Malware, Security                    |
+-----------------------+--------------------------------------+

| 

Zeek
----

Zeek is a powerful framework for network analysis and security
monitoring.

(Zeek is the new name for the long-established Bro system. Note that
parts of the system retain the “Bro” name, and it also often appears in
the documentation and distributions.)

+-----------------------+----------------------------------------+
| **SBB License**       | GNU General Public License (GPL) 2.0   |
+-----------------------+----------------------------------------+
| **Core Technology**   | C                                      |
+-----------------------+----------------------------------------+
| **Project URL**       | https://www.zeek.org/                  |
+-----------------------+----------------------------------------+
| **Source Location**   | https://github.com/zeek/zeek           |
+-----------------------+----------------------------------------+
| **Tag(s)**            | IDS, Security                          |
+-----------------------+----------------------------------------+

| 
| End of SBB list
