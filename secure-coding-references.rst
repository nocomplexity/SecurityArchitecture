Secure Coding Guidelines
--------------------------

Creating software is hard. Creating software that meets trivial security and privacy design rules has proven to be very difficult. Securing coding is the practice of developing software that prevents security and privacy risks

This section gives an opinionated list of good programming standards for creating software that meets some form of minimal security standards. When it comes to privacy standards for software it's simple: Make sure the secure coding rules are enforced and no personal data can be exposed in any way. So start with using the privacy principles before coding.

Every software engineer should use Secure Coding guidelines and practices. And every company must check that software used meets minimal standards regarding mitigating security and privacy risks.


Reproducible builds
^^^^^^^^^^^^^^^^^^^^^

Reproducible builds are a set of software development practices that create an independently-verifiable path from source code to the binary code used by computers.  Reproducible Builds project gives rules, guidelines, tools and more to allow verification that no vulnerabilities or backdoors have been introduced during the software compilation process. 

https://reproducible-builds.org/



Mozilla
^^^^^^^^

Mozilla is an OSS Foundation that produces a Browser and various other online communication tools. Security and privacy is a number one priority for the Mozilla Foundation. Mozilla produces large amount of code in various programming languages. One of the secure coding guidelines that is used internal can be found here: https://wiki.mozilla.org/WebAppSec/Secure_Coding_Guidelines


GOlang programming
^^^^^^^^^^^^^^^^^^^^

Go Language Web Application Secure Coding Practices, https://checkmarx.gitbooks.io/go-scp/
CC-Licensed so you can edit this GitBook yourself. Check the repository on https://github.com/Checkmarx/Go-SCP  
And of course OWASP Secure Coding Practices are used for this GO specific publication.

Crypto coding standards
^^^^^^^^^^^^^^^^^^^^^^^


https://github.com/veorq/cryptocoding 
This reference gives good "coding rules" for implementations of cryptographic operations, and more generally for operations involving secret or sensitive values. Created by Jean-Philippe Aumasson (https://aumasson.jp/)


Defensive Coding Guide
^^^^^^^^^^^^^^^^^^^^^^^

A Guide to Improving Software Security, http://redhat-crypto.gitlab.io/defensive-coding-guide/

This document provides guidelines for improving software security through secure coding. It covers common programming languages (C,CPP, Python, GO) and libraries, and focuses on concrete recommendations. Also lots of unix 'must do' and 'never do' tips from a security viewpoint.Licensed CC-BY-SA.



RUST programming
^^^^^^^^^^^^^^^^

Guide to develop secure applications with Rust, https://anssi-fr.github.io/rust-guide/ 

The object of this document is to provide hints and recommendations for secure applications development using the Rust programming language. This guide also includes a simple checklist.
Github repository on: https://github.com/ANSSI-FR/rust-guide 