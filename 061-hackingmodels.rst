Hacking Reference Models
=========================

This directs you to reference models for advanced hacking. 


Car Hacking
------------

Cars and especially autonomous cars are trending. Cars are nowadays also almost computers on wheels. In order to make sure it's safe, secure and vendors do not mess with your privacy hacking cars should not be a crime but should be encouraged. Since most advanced cars are build upon OSS software security and privacy has increased significantly. 

To know how secure cars are, use:

The Car Hackers Handbook: http://opengarages.org/handbook/ 
This Car Hackers Handbook will help you create better threat models for vehicles. Also your knowledge on how cars work will increase per page.

 
Robot Hacking
------------------

Robots are more and more used on various places. E.g. robots are used in homes, in assembly lines in industry and are deployed in medical facilities. But robot security is still underestimated. 

The Robot Security Framework (RSF)is a standardized methodology to perform security assessments in robotics. 
The model is GPLv3 licensed and can be found here: https://github.com/aliasrobotics/RSF

Fingerprinting
---------------------

Fingerprinting is a solid technique for retrieving information. This can be information of systems but also persons. From a privacy and security perspective knowing how easily fingerprinting is gives input for better security and privacy measurements.

Device fingerprinting or browser fingerprinting is systematic collection of information about a remote device, for identification purposes. With the ultimate goal: To identify you as person and sell you things.

Fingerprinting techniques are so good nowadays that asking for user login name with user credentials is more error prone than identifying an user by using advanced fingerprinting techniques. Fingerprinting is stateless and transparent for the user. Any third-party interested in fingerprinting can still get some piece of information of you.

Client-side scripting languages enabled in browsers (e.g. Javascript) make it possible to collect very rich fingerprints. Browser fingerprints are also called “cookieless monsters” because it is not necessary to use cookies to collect a rich fingerprint of an user. And the good news is: Detection for users is difficult, unless you have some inside information on how a company really deals with the GDPR and how they are using this gathered personal data.

Everything you use to make a network connection is vulnerable for network fingerprinting tools. E.g. TCP/IP stack fingerprinting can be used to identify types of systems and used network configurations.

Average users are of course not aware of fingerprinting techniques used. But to give you some information on what information is (easily) retrievable when you visit a web site:

* Type of browser
* Language
* Color Depth used
* Screen Resolution
* Timezone
* Information on browser session storage
* Information if a browser has IE specific ‘AddBehavior’
* CPU class of your machine
* Platform (Operating system)
* DoNotTrack settings enabled in your browser
* Full list of installed fonts (maintaining their order, which increases the entropy)
* Information on Plugins (IE included)
* Information on AdBlockers  installed
* Information if the user has tampered with its languages settings in the browser
* Information if the user has tampered with its screen resolution in the browser
* Information if the user has tampered with its OS settings
* Information if the user tampered with its browser settings
* Touch screen detection and capabilities
* Pixel Ratio
* Number of logical processors available to the user browser or device
* Device memory
* Microphone, Camera (in use, present etc)

And this list is not even complete. Storing this information or pieces of this information will expose some of your privacy. Various researchers have shown that the accuracy to identify users using only finger printing technique is highly accurate. Even better than user a password or two phase authentication. 

Using tools like Fingerprint2 (see `OSS Privacy Applications. <http://security-and-privacy-reference-architecture.readthedocs.io/en/latest/12.2-oss-privacy-productslist.html>`_) within your Secure Software Development Life Cycle Processes will minimize the risks that third party service providers you use for your Internet facing systems (rich websites) are a risk for your GDPR compliance efforts. If you have a good valid reason to use fingerprinting techniques to identify your users you should ask for permission from your users if you want to meet the GDPR.
