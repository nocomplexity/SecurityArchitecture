# Mozilla Security Principles

*This document defines a set of security principles that all operational
groups at Mozilla must follow. The principles are designed to reduce the
exposure of our systems and services from attackers who could gain
privileged access and compromise sensitive data.*


**Goal:** Limiting the amount of reachable or usable services to the
necessary minimum.

**Do**

-   List all services presented to the network (Internet and Intranets).
    Justify the presence of each port or service.

**Do not**

-   OpenSSH Server (sshd) is running but no users ever login.
-   A web-application has a web accessible administration interface, but
    it is not used.
-   A database server (SQL) allows connections from any machine in the
    same VLAN, even though only a single machine needs to access it.
-   The administration login panel of the network switch for the office
    network is accessible by users of the office network.

## Do not grant or retain permissions that are no longer needed

**Goal:** Expire user access to data or services when users no longer
need them.

**Do**

-   Use role-based access control (allows for easy granular escalation
    of privileges, only when necessary)
-   Expire access automatically when unused.
-   Automatically disable API keys after not having been used for a
    given period of time and notify the user.
-   Use different accounts for different role types (admin, developer,
    user, etc.) when no good role-based access control is available.
-   Routinely review user’s access permissions to ensure they’re still
    needed.

**Do not**

-   Grant global root access (e.g. via ‘sudo’) for all operation
    engineers on all systems.
-   Give access “just in case”.
-   Retain access to services that you no longer use.

## Defense in Depth

### Do not allow lateral movement


**Goal:** Make it difficult or impossible for an attacker to move from
one host in the network to another host.

**Do**

-   Prevent inbound network access to services on a host from clients
    that do not need access to the service through either host-based
    firewall rules, network firewall rules/AWS security groups, or both
    (which is preferred).
-   Clearly enforce which teams have access to which set of systems.
-   Alert on network flows being established between difference
    services.

**Do not**

-   Allow inbound OpenSSH, RDP connections from any host on any network.
-   Run unpatched container management services (e.g. Docker) or kernels
    which allow a user in one container to escape the container and
    affect other containers on the same host.

### Isolate environments


**Goal:** Separating infrastructure and services from each other in
order to limit the the impact of a security breach.

**Do**

-   In cases where two distinct systems are used to govern access or
    authorization (e.g. Okta and Duo), ensure that no single user or
    role has administrative permissions across both systems.
-   Use separate sets of credentials for different environments.

**Do not**

-   Have system administrators with access to every system/every
    service.
-   Establish service users with access to multiple services.
-   Allow tools remotely executing code on systems from a centralized
    location (single Puppet Master, Ansible Tower, Nagios, etc.
    instance) across multiple services.
-   Re-use functionality across services when not required (such as
    sharing load balancers, databases, etc.)

### Patch Systems


**Goal:** Ensuring systems and software do not contain vulnerabilities
when these are found in software over time.

**Do**

-   Establish regular recurring maintenance windows in which to patch
    software.
-   Ensure individual systems can be turned off and back on without
    affecting service availability.
-   Enable automatic patching where possible.
-   Check web application libraries and dependencies for
    vulnerabilities.

### Meet Web Standards


**Goal:** Reduce exposure to web attacks by following the [web security
standards](https://infosec.mozilla.org/guidelines/web_security).

**Do**

-   Achieve B+ or higher on [Mozilla’s
    Observatory](https://observatory.mozilla.org/).
-   Follow the [Web Security
    Guidelines](https://infosec.mozilla.org/guidelines/web_security).

### Guarantee data integrity and confidentiality

**Goal:** Ensuring data confidentiality, integrity, and authenticity is
respected throughout its lifecycle.

**Do**

-   Use full-disk encryption where available on systems without physical
    security (laptops and mobile phones).
-   Encrypt credentials storage databases (Ansible Vault, Credstash,
    etc.)
-   Encrypt data in transit with TLS (during transmission).
-   Also encrypt data in transit inside the internal network.

**Do not**

-   Terminate TLS (e.g. with a reverse proxy or load balancer) outside a
    system and then transmit the data in clear-text across the rest of
    the network.
-   Use STARTTLS without also disabling clear-text connections.

## Know Thy System

### Fraud detection and forensics


**Goal:** Inspect events in real-time in order to alert on suspicious
behavior, and store system behavior information in order to retrace
actions after a security breach.

**Do**

-   Audit and log system calls (e.g. with auditd or Windows Audit) made
    by processes when running in an operating system you control (e.g.
    not AWS Lambda)
-   Send logs off the account or system (e.g. AWS CloudTrail, system
    logs, etc.) outside of the account or system (different AWS account,
    MozDef, Papertrail, etc.)
-   Detect and alert on anomalous changes.

### Are you at risk?

**Goal:** Assessing how exposed you are to danger, harm or loss.

**Do**

-   Run [Rapid Risk Assessments
    (RRA)](https://wiki.mozilla.org/Security/Risk_management/Rapid_Risk_Assessment)
    for your services.
-   Estimate what would be the impact if your service was compromised.

**Do not**

-   Think it will never happen to you.

### Inventory the Landscape

**Goal:** Provide an accurate, maintained catalog, or system of records
for all assets.

**Do**

-   Keep an inventory of services and service owners.
-   Keep an inventory of machines (e.g. ServiceNow, AWS Config,
    Infoblox, etc.) which is updated automatically.
-   Ensure that the inventory contains IP addresses of systems in
    particular when using IPv6 (which cannot realistically be scanned).

## KISS - Keep It Simple and thus Secure

**Goal:** *KISS comes from [‘Keep It Simple,
Stupid’](https://en.wikipedia.org/wiki/KISS_principle). You can only
secure a system that you can completely understand.*

**Do**

-   Keep things simple. Prefer simplicity over a complex and specific
    architecture.
-   Ensure others can understand the design.
-   Use standardized tooling that others already know how to use.
-   Draw high-level data flow diagrams.

## Authentication and authorization

### Require two-factor authentication


**Goal:** Require 2FA (or MFA) on all services internal or external to
prevent attackers from reusing or guessing a single credential such as a
password.

*MFA (multi-factor authentication, also called 2FA for two-factors) is
method of confirming a user’s claimed identity by utilizing a
combination of two different components such as something you know
(password) and something you have (phone).*

See also why:
* [Rationales\#mfa](https://infosec.mozilla.org/fundamentals/rationales#mfa).*

**Do**

-   Use an SSO (Single Sign On) solution with MFA.
-   For services that can not support SSO, use the service’s individual
    MFA features (e.g. GitHub and Google MFA).
-   Servers carrying secrets or widespread access (or any other
    potentially sensitive data) should verify the user’s identity end to
    end, such as by prompting for an additional MFA verification when
    connecting to the server, even when behind a bastion host.

### Use central identity management (Single Sign-On)

**Goal:** Minimize credential theft and identity mismanagement by
minimizing the handling of user credentials such as password, MFA to a
set of dedicated systems.

**Do**

-   Use an SSO (Single Sign-On) solution that authenticates users
    credentials on your service’s behalf.
-   Servers update their user sessions from the SSO systems regularly to
    ensure the user is still active and valid.
-   Use authorization (e.g. group membership) data from the SSO system
    (possibly, in addition to your own authorization data)

**Do not**

-   Accept, process, transmit or store user credentials (passwords,
    OTPs, keys, etc.) Let the authentication server directly handle that
    data.
-   Use direct LDAP authentication for users.

See also why:
* [Rationales\#decentralized-user-account-management](https://infosec.mozilla.org/fundamentals/rationales#decentralized-user-account-management).

### Require strong authentication


**Goal:** Use credential-based authentication and user session
management to grant access.

See also why:
* [Rationales\#shared-passwords](https://infosec.mozilla.org/fundamentals/rationales#shared-passwords),
* [Rationales\#password-reuse](https://infosec.mozilla.org/fundamentals/rationales#password-reuse).*

**Do**

-   Use credential-based authentication and user session management
    where the session information is passed by the user.
-   Use API keys for service authentication.
    -   Prefer using asymmetric API keys with request signing (e.g. x509
        client certificates, AWS Signature) over symmetric API keys
        (e.g. HTTP header) where possible.
    -   Ensure that API keys can be automatically rotated in the case of
        a data leak.
-   Use a password manager to store distinct passwords for each service
    a user accesses.
-   Use purpose-built credential sharing mechanisms when sharing is
    required (1password for teams, LastPass, etc.)

**Do not**

-   Use easy to guess passwords or vendor default passwords.
-   Send your password to other individuals.
-   Send shared passwords over email or communication mediums other than
    purpose-built credential sharing mechanisms.
-   Use the same password for multiple services.
-   Trust traffic from a certain network address.
-   Rely on VLANs or AWS VPCs to indicate requests are safe.
-   Use IP ACLs as replacement for authentication.
-   Trust the office network for access to devices.
-   Use [TCP Wrapper](https://en.wikipedia.org/wiki/TCP_Wrapper) for
    access control.
-   Use machine API keys for user authentication.
-   Use user credentials for machine authentication.
-   Store API keys on devices that are not physically secure (e.g.
    laptops or mobile phones)

**NOTE:** The “**do**” and “**do not**” used in this document are
example of controls or implementation of the principles, but do not
represent an exhaustive list of possibilities. 



The Mozilla security principles are derived from: https://infosec.mozilla.org/fundamentals/security_principles.html These principles are reviewed and edited. Original copyright and license: 2017 by individual contributors. Content available under a Creative Commons license.