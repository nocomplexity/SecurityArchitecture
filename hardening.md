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
