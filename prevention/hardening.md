# Hardening

Hardening is a process intended to eliminate a means of attack by patching vulnerabilities and turning off nonessential services.
Using hardening is a great way to make your IT less vulnerable. 

Hardening should be done for every hardware and software object. Hardening can be a lot of work. But more and more good products have good defaults. 
Choosing an already hardened software solution, like a hardened Operation System can save you a lot of work and makes you less vulernable for cyber security risks.


## Kubernetes Hardening Guidance


This guidance describes the security challenges associated with setting up and securing
a Kubernetes cluster. It includes hardening strategies to avoid common
misconfigurations and guide system administrators and developers of National Security
Systems on how to deploy Kubernetes with example configurations for the
recommended hardening measures and mitigations. This guidance details the following
mitigations:
- Scan containers and Pods for vulnerabilities or misconfigurations.
- Run containers and Pods with the least privileges possible.
- Use network separation to control the amount of damage a compromise can cause.
- Use firewalls to limit unneeded network connectivity and encryption to protect confidentiality.
- Use strong authentication and authorization to limit user and administrator
access as well as to limit the attack surface.
- Use log auditing so that administrators can monitor activity and be alerted to potential malicious activity.
- Periodically review all Kubernetes settings and use vulnerability scans to help ensure risks are appropriately accounted for and security patches are applied

This great guide is created by the US National Security Agency (NSA), Cybersecurity Directorate, Endpoint Security and the US Cybersecurity and Infrastructure Security Agency (CISA). This guide is published under a Creative Commons Attribution 4.0 license.


Link to the [Kubernetes Hardening Guidance, version august 2021](https://media.defense.gov/2021/Aug/03/2002820425/-1/-1/1/CTR_KUBERNETES%20HARDENING%20GUIDANCE.PDF)

## Linux Hardening Guide

Good hands-on guide creator by the security researcher and developer of [Whonix](https://www.whonix.org/). This guide aims to explain how to harden Linux as much as possible for security and privacy. This guide attempts to be distribution-agnostic and is not tied to any specific one.

[Link](https://madaidans-insecurities.github.io/guides/linux-hardening.html): https://madaidans-insecurities.github.io/guides/linux-hardening.html

## OpenSSH

Hardening guide and configuration guide of OpenSSH server and client. All Mozilla sites and deployment should follow this mozilla created reference guide.
Most default OpenSSH settings that are security-related already provide good security. But when good is not enough, this guide is a good start to make your configuration better.

link:[https://infosec.mozilla.org/guidelines/openssh](https://infosec.mozilla.org/guidelines/openssh)

## WordPress Hardening

WordPress is one of the most used FOSS Content Management Systems. Almost 40% of the web is powered by this great FOSS software. But when using third party plugins the risk of security vulnerabilities increased. Security in WordPress is taken very seriously so if you do not mess with the defaults and make sure you apply continues updates the risks is manageable. However if you have no good process to continuously mitigate the risks of your third party plugins you take a large risks. This guide gives you a head start to prevent security problems when using WordPress!

```{note}
This guide created by the developers of WordPress touches the basics. If you are no security experts: Ask help. But keep away from people who frame WordPress as insecure by default. Direct these so called security experts to this guide and look out for security experts who known the value of using FOSS software and have experience of mitigating threads with WordPress. 
 ```

This guide is to make sure you have a solid default WordPress configuration. 


Link: [https://wordpress.org/support/article/hardening-wordpress/](https://wordpress.org/support/article/hardening-wordpress/)