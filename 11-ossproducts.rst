Generic Security Architecture
================================


When you are aware of the advantages and disadvantages of using open source
building blocks for your security architecture or design, this reference architecture provides an up-to-date overview of really great open source security solutions. 

A known difficult task is to select (or create) solution building blocks that covers the needed functionality. Of course you should always start with principles, requirements and constraints first. And remember: No single tool will fit all use cases. So select the right tool for the right job.

To give some guidance on selecting products to lower risks on security and privacy using a generic conceptual architecture model is useful. 

The key of a useful conceptual model is that a separation is made between the needs (requirements) and the solution ('the how') is clear.

Generic Security Architecture 
---------------------------------------------

The number of FOSS security applications available to solve your problems is over
overwhelming. But for a good security architecture you should first determine WHAT must be solved before jumping into solutions. 

The following conceptual security topology helps with
arranging functional to product mapping needs:


.. image:: /Images/security-abbs.png
  

For every security or privacy function or service needed you should look
serious at using open transparent reusable solutions. So Open Source. Of
course many vendors provide good solid security products for specific
use cases. But when you feel you need a trivial security or privacy
service, there is almost always a working and maintained OSS application
available. When using OSS solutions, you have have a large choice
of companies that deliver maintenance and support on this application on
commercial bases. 


Generic Privacy Architecture
-----------------------------

Besides strong security measurements strong encryption privacy is hard to accomplish. Especially online and when you do not use FOSS software in combination with open hardware that you can really trust! However due to the growing importance privacy the number of FOSS tools available is increasing.

When searching for solutions to control privacy you should make a clear distinguish between:
- Architecture Building Blocks (ABBs) and
- Solution Building Blocks (SBBs)

In this section a generic privacy architecture is outlined. This architecture outlines WHAT must be done, so the ABBs do not yet force you into a solution.

 A generic privacy framework with relevant privacy Architecture Building Blocks:

.. image:: /Images/privacy-abbs.png

Using this privacy ABBs you can select OSS Solution Building Blocks that match your requirements. And remember: No single (OSS or commercial) is perfect. A tool alone will never be enough. So make sure you have a good balance between tool support and a good privacy and/or security organization to manage risks.
