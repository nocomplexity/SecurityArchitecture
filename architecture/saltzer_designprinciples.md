# Saltzer and Schroeder's design principles

Saltzer and Schroeder's design principles are design principles enumerated by Jerome Saltzer and Michael Schroeder in their 1975 article The Protection of Information in Computer Systems,[1] that from their experience are important for the design of secure software systems. 

The design principles:

* Economy of mechanism: Keep the design as simple and small as possible.
* Fail-safe defaults: Base access decisions on permission rather than exclusion.
* Complete mediation: Every access to every object must be checked for authority.
* Open design: The design should not be secret.
* Separation of privilege: Where feasible, a protection mechanism that requires two keys to unlock it is more robust and flexible than one that allows access to the presenter of only a single key.
* Least privilege: Every program and every user of the system should operate using the least set of privileges necessary to complete the job.
* Least common mechanism: Minimize the amount of mechanism common to more than one user and depended on by all users.
* Psychological acceptability: It is essential that the human interface be designed for ease of use, so that users routinely and automatically apply the protection mechanisms correctly.
* Work factor: Compare the cost of circumventing the mechanism with the resources of a potential attacker.
* Compromise recording: It is sometimes suggested that mechanisms that reliably record that a compromise of information has occurred can be used in place of more elaborate mechanisms that completely prevent loss.

*([source Wikipedia](https://en.wikipedia.org/wiki/Saltzer_and_Schroeder%27s_design_principles) )*

## Least privilege

* Each user and program should operate using fewest privileges possible
* Limits the damage from an accident, error, or attack
* Reduces number of potential interactions among privileged programs
* Unintentional, unwanted, or improper uses of privilege less likely
* Extend to the internals of a program: only smallest portion of program which needs those privileges should have them

## Economy of mechanism/Simplicity

* Protection system's design should be simple and small as possible
* “techniques such as line-by-line inspection of software and physical examination of hardware that implements protection mechanisms are necessary. For such techniques to be successful, a small and simple design is essential.‘”
* Aka “KISS” principle (``keep it simple, stupid'')

## Open design

* The protection mechanism must not depend on attacker ignorance
* Instead, the mechanism should be public
Depend on secrecy of relatively few (and easily changeable) items like passwords or private keys
* An open design makes extensive public scrutiny possible
* Makes it possible for users to convince themselves system is adequate
* Not realistic to maintain secrecy for distributed system
* Decompilers/subverted hardware quickly expose implementation “secrets”
* Even if you pretend that source code is necessary to find exploits (it isn't), source code has often been stolen and redistributed

* Claude Shannon (inventor of information theory) restated Kerckhoff's Law as: “[Assume] the enemy knows the system”

This is one of the oldest and strongly supported principles, based on many years in cryptography
Kerckhoffs's Law: “A cryptosystem should be designed to be secure if everything is known about it except the key information”


## Complete mediation (“non-bypassable”)

* Every access attempt must be checked; position the mechanism so it cannot be subverted. For example, in a client-server model, generally the server must do all access checking because users can build or modify their own clients

## Fail-safe defaults (e.g., permission-based approach)

* The default should be denial of service, and the protection scheme should then identify conditions under which access is permitted
* More generally, installation should be secure by default

## Separation of privilege

Ideally, access to objects should depend on more than one condition, so that defeating one protection system won't enable complete access

## Least common mechanism

* Minimize the amount and use of shared mechanisms (e.g. use of the /tmp or /var/tmp directories)
* Shared objects provide potentially dangerous channels for information flow and unintended interactions

## Psychological acceptability / Easy to use

The human interface must be designed for ease of use so users will routinely and automatically use the protection mechanisms correctly
Mistakes will be reduced if the security mechanisms closely match the user's mental image of his or her protection goals
