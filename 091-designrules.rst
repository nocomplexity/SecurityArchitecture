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
