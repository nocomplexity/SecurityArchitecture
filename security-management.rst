Security Management
---------------------

Security is just not an IT technology challenge. Security is in the end a business issue that must be addressed managed and controlled. So people, processes, and technology(FOSS Tools). 

Reuse of security control and management frameworks has a number of advantages:

- It saves time (and costs).
- You can easily adjust and improve a good framework for your specific situation.
- Special Security (FOSS)tools are available that are designed that make managing and controlling easier. 

In order to control security and privacy risks, you should be able to apply needed technical security and privacy policies for all your systems, and monitor your systems to ensure they remain compliant with the approved settings. The best way to manage this complex challenge is to automate.

Using automation a necessary step for security and privacy. Good automation tooling has the capability to apply security and privacy settings for all your IT components in a simple, consistent, manner. And you far better control in a large complex IT environment. This since there is often a single point of truth where all settings are stored and managed.

Good automation tooling has the capability to apply security and privacy settings for IT components in a simple, consistent, manner. A single point of truth where all settings are stored and managed offers advantages for managing and reporting. But be mind: Not in call use case using centralized tooling are a good choice. The principle of separation of concerns also applies for designing a security solution architecture. 

A number of (FOSS) tools have proven to be usable for automating security and privacy settings for all kinds of IT components:

-    Ansible: Ansible (https://github.com/ansible/ansible)  allows you to simply define your systems settings for security. Ansible works with a Playbook syntax that allows you to define security settings for any component in a IT landscape. E.g.  firewall rules, users and groups, or applying custom security policies for applications.

-   OpenSCAP (Open Source Security Compliance Solution). The SCAP (https://www.open-scap.org/) is a specification for expressing and manipulating data in standardized ways. SCAP uses several individual specifications in concert to automate continuous monitoring, vulnerability management, and security policy compliance evaluation reporting. The Security Content Automation Protocol (SCAP) is U.S. standard maintained by National Institute of Standards and Technology (NIST). The OpenSCAP project is a collection of open source tools for implementing and enforcing this standard.
-    Open Policy Agent (OPA). The Open Policy Agent (OPA - https://www.openpolicyagent.org/ ) is an open source, general-purpose policy engine for Cloud environments that enables unified, context-aware policy enforcement across the entire stack. OPA provides a high-level declarative language for authoring policies and simple APIs to answer policy queries. Using OPA, you can offload policy decisions from IT services.
-    SaltStack. SaltStack (https://repo.saltstack.com/ ) makes software for complex systems management at scale
-    InSpec. InSpec (https://github.com/chef/inspec)  is a free and open-source framework for testing and auditing your applications and infrastructure. InSpec works of course nice together with Chef(https://www.chef.io/) . Chef is an automation language and tool for deployment to define your infrastructure as code.

Security and privacy is a complex field. So there is no silver bullet solution for managing and controlling. There is also no single tool that fits on all use cases. 