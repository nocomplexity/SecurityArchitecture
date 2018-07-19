*************************************
Security and Privacy designs
*************************************

In order to provide you with the best reusable information when creating your designs, this section outlines some key design blueprints.

How do I apply privacy by design
=================================
Privacy by design refers to principles that must be applied for all systems where in potential private data is captured or processed.
Article 25 of the EU General Data Protection Regulation (GDPR) states that data protection by design is mandatory. However in applying this in practice can be hard. But as with all challenges within security and privacy good design rules have been developed.

A good practical guide for implementing privacy by design is created by Enisa: https://www.enisa.europa.eu/publications/privacy-and-data-protection-by-design

A nice overview of privacy design patterns can be found at https://privacypatterns.org/patterns/


How do I manage API security
===============================

For APIs that will be able to transport private or secure information a risk assessment should be completed. Be aware that APIs are part of the whole system, but for inboud or outbound APIs examing the information that will be transported by an API is a good start. 

API Provider security controls are typically provided by a proxy or api-gateway. This because all traffic towards API end points is than centrally managed. You can of course also decentralize this, but than make sure all containers configurations are automatically provisioned. Minimum API controls should be:

- API key Authorisation (*) 
- OAuth Authentication (*)
- Request Rate Limiting
- Logging & Realtime Analytics
- Threat Protection
- Transport Security
- Good API key security requires use of a vault.
- Established continuous code review processes
- Use of a ‘soft identifier’ or tag to enable tracking and analytics of the API

(* if you offer protected services)

How do I validate a password?
=================================

A common way to validate the password strength is to check it against dictionaries.
If you want to take your password validation to the limit there are multiple list in the open domain available that you can use.

A nice collection of password lists can be found at: https://github.com/danielmiessler/SecLists/tree/master/Passwords 

In this passwords directory you can find a number of password lists that can be used by multiple tools when attempting to guess credentials for a given targeted service.

What are good privacy design patterns?
=========================================

A nice and proven way to speed up creating a privacy architecture or design challenges is to use design patterns.  Good reusable solutions for applying ‘Privacy-by-design’ in your architecture and implementation activities can increase the speed of creating and improve the quality of your IT solution. However many documents that have a title ‘Privacy-by-design’ and claim to help you with this architecture challenge do little more than giving a summary of all the GDPR rules and principles that must be taken into account. So these kind of documents give you little help when you are looking a way for speeding up your ‘Privacy-by-design’ challenge.

Privacy patterns can be regarded as partial solutions to common privacy problems. So when you are facing privacy design challenges a good way is to find a number of good small solutions and glue these together.

A very good and rich collection of privacy design patterns can be found on: https://privacypatterns.org/patterns/  E.g. you can find here privacy design patterns for:

* Masquerade
* Use of dummies
* Data Breach Notification Pattern
* Layered Policy Design
* Strip Invisible Metadata and many more!

All these patterns are developed as mini ‘design solutions’ to common privacy problems. Using these privacy patterns is an easy and practical way to solve ‘privacy-by-design’ challenges within small and large organizations. 

Adding new privacy patterns to this collection is open for all, since this ‘Privacy Patterns’ project is an open project. Check https://github.com/privacypatterns if you want to contribute.

This document is a reference to open security and privacy information to speed up creation of solution architectures. So the https://privacypatterns.org/patterns/ is the open resource to look for privacy patterns. This site has a nice friendly UX what minimize the time needed for finding the right privacy pattern.



