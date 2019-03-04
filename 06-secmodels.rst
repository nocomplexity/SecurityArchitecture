Security and Privacy models
============================

Introduction
------------

The essence of information security is to protect information. It is
just that simple. So whenever possible do not make it more complicated
than needed. Complexity for cyber security and privacy arise when
information needs to be shared or must be made accessible by some
digital device. The world where information was only available in
physical archives is long gone. The focus from physical information
security is shifted to cyber information security. But be aware: Crucial
principles of centuries of physical information protection are still
valuable today. Especially principles related to the intangible soft
issues when information is shared. Ever wondered how some organizations
managed to keep their valuable information secret for many decades?

Information protection is needed against unauthorized access, use,
disclosure, modification or destruction. That means several security
measures are needed to protect information from unauthorized viewers.
Measures can be implemented by procedural, physical or with complex IT
tools. But before classifying and creating or finding good measures it
is essential that the problem field is made clear.

Creating effective solutions for information security problems can be
done by creating a model of the problem situation. Within a model all
elements that relate with the problem situation are brought together to
study effective solutions. Without going into detail on system science
or problem solving theory: in general systems consist of sub-systems,
objects, functions or processes, and activities or tasks.

The key in creating a good model to solve a specific information
security problem is to model the problem, not the complete system with
all elements. This because modelling the world completely is
ineffective, time consuming and it does not give a direct answer to
solve a problem situation. It is far better to start with a small model
of a problem and create extensions on this model if needed.

The field of modelling problem situations to solve information security
problems is not new. Many models in literature exist. Reusing a good
model can save you time and safeguards you from making mistakes. A
prerequisite is that you start with a good model that can be trusted and
is intensively reviewed by large numbers of subject matter experts.

There are many good security models that can assist in creating a
solution architecture to solve a specific security problem for an
organization. Mind that a model can be expressed in many different
forms. E.g.:

-  One or more images;
-  Text;
-  Software model

Within the field of modelling a distinction can be made between ‘hard’
and ‘soft’ models. Hard models are often mathematical (risk) models
whereas soft models are more quality based models. Since using hard
models often gives a false sense of reliability and requires full
insight of all assumptions made it is more productive to reuse soft
security and privacy models. When creating solution architecture, you
need:

-  A threat model (what are the threats your solution gives protection
   against)
-  Insight in commonly used attack vectors. This means you need to have
   some view on the attack vectors used in the use case? 

.. image:: /Images/image_4_essenceofIS.png

Creating a good security or privacy design or architecture means you
never ever start with selecting tools for solving your problem!
Selecting tools should be the last phase of your security or privacy
design phase. You select tools when it is clear that the tool will
support in solving your security or privacy problem. Tools alone are
never enough to solve security or privacy problems. You need to fit in
tools within your security and privacy processes. Several problems exist
with many IT security tools that will hit you when you start too soon
with the solutions instead of a thorough problem diagnosis and solution
design. Wrongly selected security and privacy tools give the following
issues:

-  High costs;
-  Complex challenges to implement and manage;
-  Daily administration of a chosen tool set requires significant IT
   effort while it remains unclear if the tools are effective in
   reducing security risk;
-  Overlap in functionality of security application landscape. More is
   not always better. To be able to justify the application of security
   tools for your problem a context specific security architecture
   should give input to the following questions:


   -  What is protected with what?
   -  What are the main threats we need protection against?
   -  What is not protected by information security policies or tools?
   -  What is in scope or out of scope for your security architecture?
      E.g. business continuity management, safety management, financial
      risk management, daily IT operations, physical (building) security
      etc. In the end everything has a relation with information
      security, but you cannot cover all business aspects using an
      information security architecture document. The key is to focus
      and keep the scope clear or else complexity will become
      overwhelming.
   -  What architecture or design decisions have been made and must be
      validated explicitly?
   -  What is the model of your protection? It is far more easy to
      evaluate and improve a model, than adding new or improved security
      products continuously. Make sure that within operational security
      management processes learning and improving are key periodic
      targets.
   -  Does the security model cover all crucial security and privacy
      principles and requirements?
   -  Are the residual risks when this solution acceptable for the key
      stakeholders?

IT security in general is seen as a complex problem field, due to the
many technical and nontechnical aspects involved. Since 100% information
security is impossible, being able to qualify risks is crucial in
getting an accepted level of security protection. Good modelling helps
you to qualify security and privacy risks.

In general, it is far more easy to reuse proven concepts and models when
creating your own security model. This way you build on the work of
others and using a good model reference will reduce the risk of making
crucial mistakes.

This section covers some commonly used models and elements that can be
reused when creating a solution for a specific information security
problem.

Elements that are presented are attack vectors, some examples of
security personas and some great security models that can assist you
when creating your security design.

Common attack vectors
---------------------

Good security is goal oriented. Good security architecture is tailored
to your situation.  When defining a product or new (IT) service one of
the key activities is to define your specific security requirements.
Defining requirements is known to be hard, time consuming and complex.
Especially when you have iterative development cycles and you do not
have a clear defined view of your final product or service that is to be
created.

Defining attack vectors within your security requirements documentation
is proven to be helpful from the start. Attack vectors will give more
focus on expected threats so you can start developing security measures
that really matter in your situation from the start.

Attack vectors are routes or methods used to get into information
systems. Attacks are the techniques that attackers use to exploit the
vulnerabilities in applications. Many attack vectors take advantage of
the human element in the system or one of the maintenance activities
defined for the system, because that’s often defined as the weakest
link.

Within the IT cyber security world many terms and definitions are used.
Attack vectors usually require detailed knowledge to judge whether the
vector is relevant in a specific situation.

Some attack vectors apply to critical infrastructure components, like
NTP or DNS. E.g. in a rogue master attack, an attacker causes other
nodes in the network to believe it is a legitimate master. Contrary to
spoofing attacks in the Rogue Master attack the attacker does not fake
its identity, but rather manipulates the master election process using
malicious control packets.

The good news is: The number of possible attack vectors is limited. The
bad news is: The ways an attack vector can be exploited is endless.
Unless decent security measures are taken to minimize attacks using this
specific attack vector. Good designed security solutions are not that
complicated and complex after all. 

Common attack vectors are:

-  Analysis of vulnerabilities in compiled software without source code
-  Anti-forensic techniques
-  Automated probes and scans
-  Automated widespread attacks
-  Client validation in AJAX routines
-  Cross-site scripting in AJAX
-  Cryptographic Performance Attacks
-  Cyber-threats & bullying (not illegal in all jurisdictions)
-  DoS Attacks
-  Email propagation of malicious code
-  Executable code attacks (against browsers)
-  Exploiting Vulnerabilities
-  GUI intrusion tools
-  Industrial espionage
-  Internet social engineering attacks
-  Malicious AJAX code execution
-  Network sniffers
-  Packet Manipulation
-  Packet spoofing
-  Parameter manipulation with SOAP
-  Replay Attack
-  RIA thick client binary vector
-  Rogue Master Attack
-  RSS Atom Injection
-  Session-hijacking
-  `Side-channel attack <https://en.wikipedia.org/wiki/Side-channel_attack>`_
-  Sophisticated botnet command and control attacks
-  Spoofing
-  Stealth and other advanced scanning techniques
-  Targeting of specific users
-  Web service routing issues
-  Wide-scale trojan distribution
-  Wide-scale use of worms
-  Widespread attacks on DNS infrastructure
-  Widespread attacks using NNTP to distribute attack
-  Widespread, distributed denial-of-service attacks
-  Windows-based remote access trojans (Back Orifice)
-  WSDL scanning and enumeration
-  XML Poisoning
-  XPATH injection in SOAP message

It is recommended that you specify in your solution architecture the
attack vectors that apply to your use case. Remember to put the
explanation of the attack vectors used in an appendix, since not all
your stakeholders will know what e.g. ‘Spoofing’ is. 

Hosting, hardware, firmware and other invisible threats
-------------------------------------------------------

Computer security has become much harder to manage in recent years. This
is due to the fact that attackers continuously come up with new and more
effective ways to attack our systems. But also the emerging trend of
Cloud Computing created an extra level of complexity within the field of
cyber security and privacy protection.

A commonly wide spread fad is that Cloud Hosting is more secure than on
premise. The truth is that it is different. Security principles and all
attack vectors still apply. The main factors that make Cloud hosting
more complex to manage are:

-  Less control

-  Technical insight in exact physical and IT security measures are
   often unknown.

-  Influence and control on continuous operational changes on the cloud
   hosting facilities are not transparent for cloud consumers.

-  Trust plays a great role. You must have trust in audit and security
   reports created by a third party. The advice is to obtain always a
   right to perform a security audit yourself, but at large cloud
   hosting providers this is often not allowed.

Whether you use Cloud hosting of host your computer services still on
your own data centre all hardware threads still apply.

Since true open source hardware is still seldom seen, currently your
valuable information is vulnerable due to the following more hardware
related attack vectors:

-  BIOS attacks. BIOS is always written to a non-volatile storage device
   such as an EEPROM

-  Firmware attacks

-  Physical device tempering. Mostly done by rewiring CPU’s, CPU boards.
   Famous are of course the attacks on Crypto Devices (HSM’s) but since
   hardware tempering on normal hardware is so easy you seldom hear how
   easy hacking on ‘standard’ computer hardware devices is.

-  Physical data centres. Your data is not (never) secure in a cloud you
   do not control or manage.

An attack vector that many people forget to consider is the boot process
itself which is almost completely controlled by the BIOS.

When you are still in control of your own computer hardware, consider to
overcome the malicious attacks on BIOS by one the following methods:

-  Digital Authentication Method

-  Rollback Prevention Method

-  Physical Authentication Method

Threads related to hardware are often invisible. This does not mean they
don’t exist. Since computer hardware is seldom open, many threads are
still not widely known. In order to protect your core information you
should always take measures to be able to reduce the likelihood of
getting targeted by attack vectors that are hardware related. Many
examples exist of poor designed CPU’s, firmware, network devices,
storage devices etc. with offers great opportunities to attackers.

Security Personas
-----------------

Humans are the most important threat to security and privacy.

One of the tools of IT architects and UX designers is to work with so
called ‘Personas’. Personas are fictional characters created to
represent the different user types that might use a system, website,
product or service. Using personas is common practice when dealing with
UX design. But when developing a security architecture for a new system,
service or website security personas are also valuable to use. Security
Personas force you to think different about the goals and behaviour of
attackers that are going to hit your system.

Security Personas identify the user motivations, expectations and goals
responsible for driving bad behaviour. Of course not all personas will
behave bad on purpose. Sometimes mistakes on the use of the system or
social engineering will affect the way a persona can compromise your
system.

Benefits of Personas
^^^^^^^^^^^^^^^^^^^^^

Personas help to focus and help to make design decisions concerning IT
components by adding a layer of real-world consideration to the
conversation. They also offer a quick and inexpensive way to test and
prioritize those features throughout the development process. In
addition, they can help:

-  Stakeholders and management to discuss architecture building blocks
   to protect your system.

-  Information architects develop informed secure wire-frames knowing
   possible interface behaviour.

-  System security engineers/developers to decide which approaches to
   take based on user behaviours.

-  Testing

For security personas it is good to outline:

-  Demographics such as age, education, ethnicity, and family status.

-  The goals and tasks they are trying to complete using the system (or
   website),

-  Their physical, social, and technological environment.

-  Responsibilities: As implemented in future Identity and access
   management system, but also the formal organization responsibilities
   belong to the role within the organization.

Defining security personas is not hard. Some examples of security
personas:

-  Employee

-  Visitor (in person)

-  Internet visitor (web)

-  Administrator

-  Manager

-  Director/CEO

-  Angry customer

-  Competitor/rival

-  Neighbours

Use security personas in your security architecture so the proposed
security measures can be designed more in depth and evaluated since the
security personas are part of your security model. The list given in
this section can be used as starting point to expand the personas for
your context more in depth.


.. Sub Section for Thread Models

.. include:: threadmodels.rst 




Security Models
----------------

NIST Security framework
^^^^^^^^^^^^^^^^^^^^^^^^^

Whenever you feel the need to draw a process regarding security or risk
processes: resist the temptation! The US based NIST organization is a
well-known governmental organization that offers great publications on
all thinkable subjects regarding security.

One of the simplest, yet most frequently model is displayed here below.

.. image:: /Images/image_6_NIST.png

On the NIST site (see references) you can find in-depth information
regarding all sub functions of this security framework. The experience
is, is that it is far better to check what in your use case needs
special attention. If you ever feel the need to create your own security
framework, think again. In essence all come down to the high level
framework described by the NIST organization. Using a broad used
security framework has a number of advantages:

-  Easier communication with stakeholders;

-  Easier knowledge and experience transfer between security experts of
   different organization;

-  Saves time, time you can use to solve the real context specific
   issues regarding practice use and implementation of the security
   functions.



NIST Cloud Computing Security model
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Sooner or later you will be creating a solution or privacy architecture
where cloud hosting plays a significant part. The NIST cloud computing
security reference model is a very good model to use as reference. 

.. image:: /Images/image_12_Nist_CloudSecurityREFmodel.png


Jericho Security Model
^^^^^^^^^^^^^^^^^^^^^^^

The Jericho(tm) Security architecture model is built upon principles.
The advantages of using the Jericho model for security are:

-  A security architecture model built upon the Jericho conceptual model
   is built around maintaining flexibility and protects the most
   important security objects for the stakeholders.

-  Integration: Easier to build secure processes with other companies
   and trusted partners.

-  Simplifies use of public networks and cloud solutions

-  Aimed for use of open principles and open solution building blocks.


.. image:: /Images/image_7_Jericho.png

Unfortunate the Jericho framework is not a real open security framework.
It is copyrighted by the open group (see references chapter for more
information on this model). There are trademarks involved and all
publications are copyrighted. However due to the work of many we can
make use of the developed knowledge within the Jericho working group.
The Jericho Forum®, a forum of The Open Group, was formed in January
2004 and is no longer active. However, the approach of this forum
towards security is still alive.

Security Architecture Landscape (OSA)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Thanks to the Open Security Architecture (OSA) group there is a real
open security landscape (http://www.opensecurityarchitecture.org/). All
OSA material is CC by sa licensed, which means you can freely use and
improve it.

Below is the OSA Security architecture landscape:

.. image:: /Images/image_8_OSA.png

Source: OSA (http://www.opensecurityarchitecture.org)

The OSA Security architecture is based on patterns. Which mean for every
pattern defined the aim of the community was/is to develop a
standardized solution description. Unfortunate the OSA community is not
very active anymore, so all IT security patterns around cloud are not
yet incorporated.

For a number of reasons we have chosen not to use patterns in this
security and privacy reference architecture. However in some cases using
patterns can give an advantage. (See the Introduction, section 'What
about security patterns?' for more information).


Software Assurance Maturity Model (SAMM)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Software Assurance Maturity Model (SAMM) is an open framework to
help organizations formulate and implement a strategy for software
security that is tailored to the specific risks facing the organization.
SAMM is useful resource if you are working on a process architecture
that is needed to control all kind of aspects of software security. Our
advice is to take the processes as defined in SAMM as point of departure
within your security process design documentation. Formulating processes
yourself in not productive, so use this valuable source of information
instead of reinventing the wheel.

To get the baseline situation of your security process architecture fast
in scope, you can use a SAMM self-assessment test (see APPENDIX). Using
a self-assessment test you can get a very quick overview on the status
of the IT security processes within your organization. SAMM is an OWASP
project.

SAMM will aid in:

-  Evaluating an organization’s existing software security practices

-  Building a balanced software security assurance program in
   well-defined iterations

-  Demonstrating concrete improvements to a security assurance program

-  Defining and measuring security-related activities throughout an
   organization

As an open project, SAMM content shall always remain vendor-neutral and
freely available for all to use.

 
.. image:: /Images/image_9_SAMM.png

Source: OWASP

Reuse of the SAMM process and usage should be encouraged. This OWASP
project is like all OWASP projects a real open project. All content is
available under a Creative Commons License (by-sa). If you want to
improve this SAMM framework, OWASP is a real open foundation where
everyone can participate without borders. Also all communication and
collaboration is truly open.

The SAMM model was first aimed at evaluating the status of software
security within an organization. However due to the use in practice the
framework can also be used to improve many other aspects surrounding
security and privacy.


Security within the SDLC process
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The view below (source OWASP) is a model of how security fits into the
SDLC (Software Development and Lifecycle) process. Within almost every
solution architecture you should take the SDLC into account to position
where your solution fits and how maintenance is positioned within the
SDLC phases.

.. image:: /Images/image_10_SDLC.png

Security and privacy should be embedded in the SDLC process. Always. The
OWASP conceptual model of the (simplified) SDLC chain shows on high
level where security activities hit the SDLC process.


Car Hacking
^^^^^^^^^^^^^^^^
Modelling how things really work is the best start for good protection. So any investment or use of real world hacking modles will improve your security design.

Cars and especially autonomous cars are trending. Cars are nowadays also almost computers on wheels. In order to make sure it's safe, secure and vendors do not mess with your privacy hacking cars should not be a crime but should be encouraged. Since most advanced cars are build upon OSS software security and privacy has increased significantly. 

To know how secure cars are, use:

The Car Hackers Handbook: http://opengarages.org/handbook/ 
This Car Hackers Handbook will help you create better threat models for vehicles. Also your knowledge on how cars work will increase per page.

 
Robot Hacking
^^^^^^^^^^^^^^^^^^^^

Robots are more and more used on various places. E.g. robots are used in homes, in assembly lines in industry and are deployed in medical facilities. But robot security is still underestimated. 

The Robot Security Framework (RSF)is a standardized methodology to perform security assessments in robotics. 
The model is GPLv3 licensed and can be found here: https://github.com/aliasrobotics/RSF



Privacy Models
-----------------

When developing a privacy architecture it makes sense to investigate if audit and control functions for privacy can be combined with security services and processes that are already in place. Below some models that are designed from a privacy perspective only.


Privacy Management Reference Model(PMRM)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Privacy Management Reference Model and Methodology (PMRM) of the OASIS group can help you with:

- Analysis the impact of new privacy use cases for your company.
- Designing operational privacy management services.
- Improving services that need to be compliant with the GDPR.
- Determining use and requirements of security services from a privacy view point.
- Gives input for developing a privacy solution architecture.

When developing a privacy architecture it makes sense to investigate if audit and control functions for privacy can be combined with security services and processes that are already in place.


This model is particularly relevant to evaluate use cases in which
personal information (PI) flows across regulatory, policy,
jurisdictional, and system boundaries.


.. image:: /Images/privacy-reference-model.png

More in-depth information regarding this model can be found on the OASIS
site (see references).

Privacy Management Model
^^^^^^^^^^^^^^^^^^^^^^^^^

A privacy management model outlines how management the various processes needed for privacy can be categorized.

.. image:: /Images/privacymanagement.png

Based upon the key processes in every solution architecture a view of the various processes should be outlined. With the use of an process overview topology it is easier to map overlap between privacy, security and general IT and risks processes and departments.



