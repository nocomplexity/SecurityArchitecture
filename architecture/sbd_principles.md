# Security by Design Principles


:::{important} 
Security by Design principles do not guarantee security. They are a mandatory aid to thinking, not a replacement for it.
:::

When embracing the Security by design approach you must embrace at least the following principles:

:::{admonition} Minimise attack surface area
:class: note, dropdown
Remove unnecessary features, endpoints, and entry points.
:::


:::{admonition} Establish secure defaults
:class: note, dropdown
Default configurations should be secure out of the box (e.g., deny by default).
:::


:::{admonition} Least privilege 
:class: note, dropdown
Every component and user should have only the minimum privileges necessary to function. (Keep once, not twice.)
:::

:::{admonition} Separation of duties (and privilege)
:class: note, dropdown
No single person or process should have excessive authority; split critical functions across multiple actors.
:::


:::{admonition} Defence in depth 
:class: note, dropdown
Layer multiple, independent security controls so that failure of one does not lead to system compromise.
:::

:::{admonition} Fail securely
:class: note, dropdown
When a system fails, it should default to a closed (deny) state, not an open (allow) state.
:::



:::{admonition} Complete mediation
:class: note, dropdown
Every access request must be checked against authorisation rules, without relying on cached decisions.
:::



:::{admonition} Economy of mechanism (Keep it simple!)
:class: note, dropdown
Keep security-critical designs as simple and small as possible.

This principle is also known as: 

**Simplicity is better than complexity.**

Security mechanisms should be as simple and small as possible. Complex systems have more vulnerabilities, are harder to verify, and increase the attack surface.


A complicated solution often fails because:

- It's harder to review. No one can fully understand all the interactions.

- It's harder to configure correctly. Admins will make mistakes.

- It's harder to maintain. Fixing one bug often creates two more.

- It often relies on "security by obscurity." The complexity feels secure because it's hard to understand, but that's an illusion.
:::


:::{admonition} Open design (Avoid security by obscurity)
:class: note, dropdown
Security must not depend on secrecy of the design or implementation (security by obscurity is explicitly avoided).

This means the architecture, design and software used should be fully transparent. Assume that bad actors have access to the software and crucial documentation. 
:::


:::{admonition} Zero Trust (Don’t trust services)
:class: note, dropdown
Never implicitly trust internal or external services; verify everything.
:::


:::{admonition} Compartmentalisation
:class: note, dropdown
Isolate components so that a breach in one area does not compromise the whole system.
:::



:::{admonition} Protect data everywhere
:class: note, dropdown
Data must be protected at rest (storage), in transit (network) and when 'in-use' , so when processed at CPU level or touched by applications. So critical data should be even protected when applications perform actions on it. So data should always be encrypted. 
:::


:::{admonition} Design for secure updates
:class: note, dropdown
Systems must be able to receive and apply security patches safely and reliably.
:::


If you think a principle is not applicable for your situation: **Think again.** Or better write down your motivation and ask for an expert review on your motivation.
