Introduction
============

In our opinion security is a process, not a destination to arrive at.
Good security design and implementation takes time, patience and hard
work to achieve and maintain. You should always start with the basics by
creating an architecture or overall design. As security and privacy will
always be one of the most important subjects within IT the importance of
good security and privacy will keep growing since companies will be even
more depending on IT. Also the influence of IT will go deeper into our
lives. Next to safety security and privacy will become more important
when we realize the potential risks that come with new IT technologies.

This reference architecture is created to improve security and privacy
designs in general. In our opinion it is time to stop reinventing the
wheel when it comes down to creating architectures and designs for
security and privacy solutions.

The reference architecture is not just another security book. Since
libraries and book stores are filled with decent books on security and
privacy we wanted to create a book that is all about reuse. There are
two main pillars that drive this publication:

-  Enabling reuse for companies of all sizes worldwide in order to
   design security and privacy solutions
-  Creating an open reference architecture that enables collaboration
   and improvement in an easy way.

This reference architecture aims to enable you to create better and
faster security and privacy solutions by reusing the content provided in
this eBook. And to encourage collaboration on this eBook / reference
architecture we created this reference architecture under an open
license. We have chosen to use the Creative Commons
Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license. We know
you like credit if you contribute to a publication. If you contribute
you will of course be mentioned in all updates of this publication that
follow. And since it is a true open license, your rights regarding this
publication are no different than ours or other contributors.

To summarize this eBook is an open reference architecture aiming to help
you to design better secure systems in less time and with less cost.

Why another reference architecture
----------------------------------

Open publications for IT security and privacy are still rare. Despite
the great work of the OWASP foundation many IT security  organizations
are not that open. 

When you create a new medicine that can and will save millions of human
lives it is not only ethical but also a moral right that people can use
it. Science is there so we can build on each other’s ideas. 

This means progress for all. We all win. Within the field of software
coding Open Source (OSS/FOSS) is becoming the new de facto model. Why
create something anew that you already have created?

Within the field of security consultancy and security architecture Open
is not (yet) the de facto standard. Of course some key assets as
passwords or personal data should never be accessible. But creating
security architectures and security designs is by many positioned as an
art. That is strange of course. If you need a new color on your wall you
do not call an artist, but a painter. The same goes for security: go for
a proven open solution that has been used before. All solutions are of
course mostly always context specific. No organization is the same. But
that does not mean that every aspect for your architecture, and design
should be new. We all use standard solutions where possible. Reuse of
architecture and design is rare at the least. This reference
architecture is aimed at enabling reuse of parts that are needed in
every security architecture and design. That means less art, but the
puzzle that remains is more interesting to solve. Since this is the real
context related problem!

Availability of good references with solid reusable information makes
creating security architectures easier and more fun. Easier because when
you have a good security reference architecture you do not need various
books to find out what already good proven parts for your architecture
could be. More fun because you have more time to figure out what the
best solution for your unique security challenge is. And we see thinking
and resolving real security issues as fun. Minimizing security and
privacy risks  is always unique and context depended. E.g. unique
stakeholders, different security control system (organization) and a
different way of dealing with risks. 

Why security and privacy
-------------------------

Privacy is getting more and more important. New technologies make our
lives better but put our freedom and privacy under pressure. Terrorist
and (cyber) criminals can be more easily detected by analyzing large
amounts of data. Also ‘diseases’ can be better cured using more data of
more people.

Currently great improvements come at a large price: Big data analytics
systems are going over your user data and user data traces (e.g. mouse
movements in web pages, location data) multiple times a day. Companies
know better what you need, think and eat tomorrow than you. Your
location is continuously being tracked, due to all the communication
devices you use. Using public transport cannot be done anonymously
anymore while cars are full of track and tracing technology.

When privacy is designed first just as security we should have less
concern on security and privacy hacks. Also if more IT designs are open
and published under an open license chances of mistakes in architecture
and design will be less. Partly due to pressure of openness but also
since more experts can contribute to lower security and privacy risks
concerned with public or private systems. Of course: Transparency of
governmental systems will be a (very) long way. Companies however see
advantages of open solutions more and more. Using open solutions, open
business models and open source software for IT. A large number of
companies exist that benefit from using open designs along with open
source software.

Many new technology companies are successful due to the fact that they
promote open (FOSS) solutions. E.g. Companies like Automattic
(https://automattic.com/), Acquia (https://www.acquia.com/) or IMatix
(http://www.imatix.com/) are all very successful due to a true GPL OSS
policy.

We know that privacy can be regarded as something totally different than
security. This is why we had some resistance with combining a reference
architecture for security with privacy ‘things’. But our research showed
that:

-  Privacy has many relations with security. Many problems are similar.
-  Privacy aspects are by far not yet taken serious into architectures
   and design the way they should be. It took decades and billion dollar
   (or euro) campaigns before security aspects were taken more seriously
   into account. And yet security is still difficult due the fact that
   doing it right gives no direct business value. Doing it wrong always
   means a true disaster for your business. And he same goes for
   privacy.
-  Security and privacy are interrelated. Without security there is no
   privacy! Never.

Since privacy and security are very much interrelated both aspects will
be outlined in this reference architecture.

 

Advantage of using this reference architecture
-----------------------------------------------

A good reference architecture saves time in many ways:

-  You can create a solution architecture based on it for your specific
   situation.
-  It enables you to speed up the process of creating a specific
   solution. 
-  It contains valuable content and general background information which
   can be used, reused or referred to.

Information security architecture is an abstraction of a design that
identifies and describes where and how security controls are used. It
also identifies and describes the location and sensitivity of both user
and application data.

This open reference security architecture aims to help you create your
context specific architecture faster and with higher quality.

This reference architecture  is designed to assist and guide architects,
security designers and developers to make better decisions and to reuse
quality architecture knowledge regarding cyber security aspects.

The purpose of this document is to reuse good security principles,
requirements and design patterns to save precious time and budgets.
Since security by obscurity is in general not a good practice, we also
provide a list of OSS security software products.

Systems built with tough privacy rules will not always guarantee that
information including valuable privacy content is secure. Since security
never is nor can be perfect a very secure system will always contain
risks concerning privacy.


Who should use this reference architecture
-------------------------------------------

The target audience for this reference architecture are security experts
and companies who can see the benefit of reuse and using open source
security building blocks. Specifically all business owners, security
architects, security designers, asset owners, software developers,
system administrators and (end) users who have a role in reducing
security risks.

Scope of this reference architecture
------------------------------------

Not all aspects of security and privacy can and should be outlined in a
reference architecture. This reference architecture is not about
teaching what security and privacy is. This reference architecture is
not about providing detailed technical information on solutions that
come across.

This reference architecture is also not a lecture book on how to design
the perfect security solution architecture. There are many resources
(books, courses, foundations) that will teach you the benefits of
creating an (enterprise) architecture and how you can embed architecture
into your agile way of working. Be aware of course that an agile way of
creating new products, systems or software gives some tension regarding
security and privacy aspects. It is difficult to add security and
privacy aspects at a later point if not done correctly from the start.
So use new trends whenever possible. But if you were to design ‘A human
mission to Mars’ important aspects like security and safety cannot wait
till later. 

Since you are reading this reference architecture, we assume you are
already aware of the complex field of security and privacy. Very
detailed books, papers and studies exist for learning what security and
privacy really is. So this reference architecture will not give you in
depth detailed background information on all security and privacy
aspects. Not from an organization point of view and certainly not from
an IT point of view. 

The scope and aim of this open security architecture is to enable you to
create better and faster security solution architectures and designs
using open reusable building blocks and standards. Within the scope of
this reference architecture are:

-  Security solution aspects, e.g. models, that must, should or could be
   reused in a security or privacy solution architecture.
-  Information that can be reused in an easy way in your context
   specific security/privacy solutions. E.g. security and privacy
   principles.
-  Criteria aspects you can reuse when selecting security solutions for
   your solution architecture.
-  (Sample) Security/Privacy Solution Building Blocks that are created
   for reuse. These SBB’s serve as example to give you a more in depth
   overview of possibilities you are maybe not familiar with.

Creating security architecture consists of the following high level
steps:

-  Dive in the business strategy and organization;
-  Gather security and privacy principles and requirements;
-  Determine important constraints that apply to your architecture or
   design. There are always constraints, e.g. time, budget, subject
   matter experts available etc.
-  Derive the architecture building blocks from your architecture or
   design. Architecture building blocks help you to scope your solution.
   Using architecture building blocks gives a clear view on (new)
   integration aspects and where completely new solutions fit in the
   total IT landscape.
-  Select (or create, buy) the new Solution Building Blocks.
   Prerequisite is of course that the functionality and technical
   constrains must be clear. Often prerequisites are derived from the
   previous design step.


.. image:: /Images/image_1_scope.png

 

Within this reference architecture we will focus on the following
subjects that you should face when creating a security or privacy
solution:

-  Principles: We will provide a reusable list of security and privacy
   principles. Since this open security and privacy reference
   architecture has an Open approach we encourage you to add your
   principles to the open data source we created to help others from
   reinventing the wheel again and by doing so they save time.
-  Solution Building Blocks: We provide a list of solid reusable
   security and privacy tools and building blocks. Of course all tools
   and building blocks are open source. One core principle is that good
   security should be open. Within this eBook a detailed outline is
   given on the question if extra risks factors are involved in using
   open source solutions.
-  Reusable architecture and design patterns for security and privacy
   problems. During the architecture and design phase threat models are
   constructed. This document contains generic threat models, since
   these are reusable. That can be improved when the model is made
   publically available.

 
.. image:: /Images/image_2_scope_withredmarked.png

 

So many aspects regarding security and privacy our not in scope of this
reference architecture.

 

What about security patterns?
------------------------------

In system design, coding and architecture you should strive to reuse
predefined patterns. A pattern is a reusable way to solve a standardized
problem. This can be in software code, design or an organization
problem.

Good patterns within the security and privacy field are rare. We did
research on available reusable patterns that can help creating security
or privacy solutions faster. Our findings are:

-  Good described reusable security and privacy solution patterns are
   rare.
-  Reusable architecture and design patterns for security and privacy
   problems are scarce. Most relevant patterns are vendor specific, so
   are targeted to the solution building block reuse aspects.
-  Use of patterns can increase complexity. Understanding pattern
   language  and semantics is important before being able to judge if
   your chosen pattern applies to the unique challenge that must be
   solved. Since libraries are written on generic problem solving
   methods (note: the golden book is still not found) some precaution
   using patterns is very healthy!
-  Developing patterns (also in a collaborative way) for a reference
   architecture takes up a lot of precious time while the practical use
   (or reuse) in a solution architecture is always questionable.

We hope good developed patterns for dealing with typical security and
privacy problems will be developed in future. Also we hope these
patterns will be developed in an open collaborative way and published
under an open license so everyone can benefit and participate. Some good
attempts have been done, so maybe time for a new OWASP project to give
it a boost.

Currently we think that when you write a good solution architecture in
which you describe your problem clearly will help to create a library of
reusable solution patterns for security and privacy. One import
constraint is that your solution architecture should be published under
an open license somewhere on the internet. In this way every
organization, security designer can benefit. Some governments already
publish their architecture documents under an open license (CC) on the
internet. This is a great way for governments to align better with
society. Everyone can see how complex digital information systems become
and can suggest improvements. Detailed configuration information is not
needed to judge the risks of security or privacy vulnerabilities.
Companies worldwide are still very anxious to benefit from the
possibilities that a more open transparent company (using open
licensing) can give.


How this reference architecture is structured
----------------------------------------------

This reference architecture is built around information that helps you
creating security or privacy solution architectures.


.. image:: /Images/image_3_outlinedocument.png

It is also built to give you reusable information in an easy to find
way. The next chapter ('`Security
Models <../Text/chapter_securitymodels.html>`__\ ') deals with models,
attack vectors and information that helps you create the threat model
you need to develop in your solution architecture.

The chapter  '`Security and Privacy
Principles <../Text/chapter_principles.html>`__\ '  presents solid
security and privacy principles. Focus is on use and reuse.  The chapter
'Using Open Source for security and privacy protection' outlines facts
to demystify common fads regarding use of Open Source and security and
privacy products. This chapter outlines how to evaluate OSS Solution
Building Blocks for security and privacy applications. The chapter 'Open
Source Security and Privacy products' presents a list of great OSS
solutions available to be incorporated into your security or privacy
solution or just to take a look at.

The appendixes will give you information on reference used, as well as
information on how you can contribute with the next version of this
reference architecture.


