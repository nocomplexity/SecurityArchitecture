Security and Privacy Principles
===============================

Every organization is different. However, when you are faced with the
challenge to create a new (IT) product or service having good principles
requirements before you start will help. Always.

We have simplified this complex but crucial step needed in every
project. In this chapter you find lists of:

-  Security principles and

-  Privacy principles 

We encourage reuse! We also encourage you to add principles or correct
these principles. In time we are aiming to create a collection of the
best e.g. 100 principles for security and privacy that can be used when
creating a specific solution architecture. A good reference architecture
should save you time when creating a solution architecture, so use or
reuse these principles from this architecture. In this way you have more
time to focus on the specific context related problems. In essence the
use or reuse of good security and privacy principles prevent you from
making crucial design and implementation mistakes in your use case. 

What are principles?
--------------------

Principles are statements of direction that govern selections and
implementations. That is, principles provide a foundation for decision
making.

Principles are used within business design and successful IT projects.

Definition:

*A principle is a qualitative statement of intent that should be met by
the architecture.*

Security architecture principles are used to translate selected
alternatives into basic ideas, standards, and guidelines for simplifying
and organizing the construction, operation, and evolution of systems.

It is important to draw an early differentiation between standards,
requirements, and principles.

-  Standards are “musts”; that is, they require compliance.

-  Requirements articulate specific needs that must be met by a specific
   solution.

-  Principles, on the other hand, are more general and serve as a
   framework for making choices by providing guidance about the
   preferred outcome of a decision in a given context.

As such, the purpose of our collected principles is to support decision
making with regard to security and privacy design within all
organizations.

The following criteria can be used to determine the quality of a
principles:

-  Understandable: Every stakeholder involved should be able to
   understand the meaning, purpose and implications of a principle.

-  Consistent with other defined (or selected) principles.

-  Aimed to the goal.

-  Usable.

Principles will guide architects, consultants and designers with
decision making. Within business design and architecture, you find many
people with strong opinions with what a good and usable principle is or
is not. Discussion is always good to get a better understanding of each
other mental maps. However, discussions on what a good security
principle is should be target on what you can do with principles. How
will principles help you and your company? Can principles help you doing
projects faster and better? Can principles prevent your company
architecture and software systems becoming the next IT over complexity
landscape?

Having security and privacy principles are a crucial foundation as they
establish the basis for a set of rules and behaviours for any
organization.

.. image:: /Images/image_17_principles.png


Principles or requirements?
---------------------------

The exact difference between what a principle is and what a requirement
is, is a long running debate. Long running debates does not make your
organization more secure. It is time consuming and in the end no one is
right. So do not fall in the trap of such a semantic discussion.

Security and privacy principles have the following characteristics:

-  Principles are general rules and guidelines.

-  Principle are often a qualitative statement of intent that should be met by the architecture.

-  Principles are guidance to help making decisions with the help of rules.

Your security and privacy design should be created based upon many
design decisions. Using (approved) principles will help.

Security and privacy requirements tend to have the following characteristics:

-  Can be SMART (https://en.wikipedia.org/wiki/SMART_criteria ) formulated. So you can test if a requirement is implemented well.

-  A requirement is more context specific than a principle. E.g. your users can have different requirements on user-friendly and secure login than users of another company.

-  Requirements can be prioritized within a project, where principles are more directly shaping an architecture or design.

Principles can be regarded and threated as requirement, but due to the
formulation requirements seldom can be directly used as generic
principle.

Although the difference between security and privacy principles and
requirements is most of the time hard to make, having requirements in
addition to principles will improve a privacy or security design.

This because using requirements leaves more room to discussion and
prioritization with direct stakeholders.

What are requirements?
----------------------

Many studies show that poor requirements are a prime cause of project
failure or insufficiency. Tools that assist you with creating good
security requirements or let you reuse security requirements are rare.
But it is crucial for good security that you start with collecting
principles and requirements before coding or buying software.

Within traditional waterfall methodologies a requirements document is
created by a business analysts and subject matter experts who would
spend significant time on creating requirements that are never complete.
Developers are often faced with challenges deadlines and have little
time to handle and implement all requirements correctly. In practice
there is simply have no time to get familiar with the real meaning and
purpose of all requirements and developers make guesses on the real goal
of requirement statements.

In most projects today, a lapse of several months would either
invalidate these requirements or miss the market window altogether.
Internet speed and agility mean that projects must be quick to market
and must evolve continuously to meet the changing needs and demands of
their users.

Common Mistakes regarding security and privacy requirements

-  Basing a solution on complex or cutting edge technology and then
   discovering that it cannot easily be rolled into the 'real world'.

-  Not prioritising the User Requirements, for example 'must have',
   'should have', 'could have' and 'would have,' known as the MoSCoW
   principle.

-  Not enough consultation with real users and practitioners.

-  Solving the 'problem' before you know what it is.

-  Lacking a clear understanding and making assumptions rather than
   asking.

Requirements gathering is an essential part of any project and project
management. Understanding fully what a project will deliver is critical
to its success. This may sound like common sense, but surprisingly it's
an area that is often given far too little attention.

Many projects start with the barest headline list of requirements, only
to find later the customers' needs have not been properly understood.

Since security and is always in the end risk based we recommend that you
prioritise your chosen requirements. We advise to use the de-facto
standard: the acronym MoSCoW.

This stands for:

-  M – MUST: have this.
-  S – SHOULD: have this if at all possible.
-  C – COULD: have this if it does not affect anything else.
-  W - WON'T: have this not now, but would like this in the future.

Requirements marked as "Won't" are potentially as important as the
"Must" category. Classifying something as "Won't" acknowledges that it
is important, but can be left for a future release. In fact a great deal
of time might be spent in trying to produce a good "Won't" list. This
has three important advantages:

#. Stakeholders/Users do not have to fight to get something onto a
   requirements list.

#. Thinking about what will be required later, affects what is asked for
   now.

#. The designers seeing the future trend can produce solutions that can
   accommodate these requirements in a future release.

Reuse of requirements provides a number of benefits, including the
following:

#. Motivation for selection of components: Requirements guide the
   selection of optimal components for reuse. When requirements are
   transferred between development efforts, the rationale behind the
   original component selection decision is made available to the system
   designer.
#. Context for reuse decisions: Requirements trace back to information
   gathered from domain experts and system users. Requirement-based
   reuse decisions are set in the context of domain processes or
   specific implementation needs.
#. Parametric constraints: Requirements come in many forms, including
   parametric constraints (i.e. the system delivered must run at speed
   x) as well as general guidelines (e.g. the system's interface should
   be user friendly) and domain tasks and processes. Parametric
   constraints allow a static evaluation to narrow the field of
   available components.

.. raw:: html

   <!-- -->

An example security requirements list:

+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| RequirementID   | Requirement Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Type             | Priority   |
+=================+==============================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================+==================+============+
| 10              | Sensitive data is not logged in clear text by the application.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Implementation   | Must       |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 20              | Database connections, passwords, keys, or other secrets are not stored in plain text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Business         | Must       |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 30              | Encryption keys must be secured.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Business         | Must       |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 40              | Privileged and super-user accounts (Administrator, root, etc.) must not be used for non-administrator activities. A secure mechanism to escalate privileges (e.g., via User Account Control or via sudo) with a standard account is acceptable to meet this requirement. Network services must run under accounts assigned the minimum necessary privileges.                                                                                                                                                                                                                                                                                                                 | Functional       | Should     |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 50              | Sensitive data is not stored in persistent cookies.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Business         | Wont       |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 60              | Sensitive data is transmitted with the HTML POST protocol. So GET is NOT used for sensitive data.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Implementation   | Should     |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+
| 70              | User ID must be unique. Passwords must be stored in irreversible encrypted form, and the password file cannot be viewed in unencrypted form. A password must not be displayed on the data entry/display device. Passwords must be at least eight characters long. Passwords must be composed of at least three of the following: English uppercase letters, English lowercase letters, numeric characters, and special characters. Password lifetime will not exceed 60 days Users cannot use the previous six passwords. The system will give the user a choice of alternative passwords from which to choose. Passwords must be changed by the user after initial logon.   | Business         | Must       |
+-----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+------------+

For this book we started collecting security and privacy requirements,
since our experience shows that all good (security)  architectures and
designs have similar (if not exact) the same requirements. Within the
appendix of this document a link to a reusable list of security and
privacy requirements on GitHub for reuse. We encourage everyone to share
created requirements. See the Appendix on how you can collaborate and
make the next version of this reference architecture with us.
