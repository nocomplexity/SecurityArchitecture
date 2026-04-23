# Python Security Applications Checklist

Python-based security applications are fundamental to modern computing; however, many currently fail to meet minimum security baselines. Deploying insecure security tools can inadvertently weaken your infrastructure rather than fortify it. Furthermore, the availability of high-quality, well-maintained Free and Open Source Software (FOSS) Static Analysis Security Testing (SAST) tools for Python remains limited. **True security relies on transparency and robustness—never on "security by obscurity".**

Use this checklist to perform a comprehensive risk assessment before adopting any security application developed in Python. It is designed to help you:

- Identify potential vulnerabilities within the tool itself.

- Evaluate code quality and maintenance standards.

- Ensure the project aligns with essential security principles.

Consistent application of this checklist will facilitate informed decision-making and mitigate the risk of introducing new vulnerabilities when using Python based security applications on your environment.



The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in RFC 2119.

A security project MUST meet the highest security quality standards. No tool is perfect, and the way a design is converted into a program is always subjective. There is no single "best" way to create and implement a design; there are always multiple options. However, there are fundamentally wrong ways to develop software that cause weaknesses and lead to vulnerabilities. This MUST be avoided in security-critical software. A security program that is relied upon MUST be inherently secure and MUST NOT introduce vulnerabilities.

There are few specific evaluation criteria that can be directly applied to evaluate Python security applications.
Transparency, comprehensive documentation, and the practice of proven security-by-design principles MUST be considered a bare minimum.

While security projects vary, the documentation MUST clearly state when a requirement is not applicable. This prevents ambiguity during security reviews and ensures users that even trivial security aspects have been addressed.
To evaluate or create Python security applications, the following minimal security requirements MUST be met:

1. **Security Policy**

A security project MUST have a security policy, such as a [SECURITY.md](https://github.com/nocomplexity/codeaudit/blob/main/SECURITY.md) file, to ensure that potential security issues can be reported securely and effectively.

+++

2. **OpenSSF Best Practices**


A security project MUST maintain an [OpenSSF Best Practices](https://www.bestpractices.dev/en) badge to demonstrate that all fundamental security requirements have been satisfied.

+++

**3. Fuzzing**


A fuzzer SHOULD be incorporated into the testing workflow where appropriate to identify unexpected behaviours or vulnerabilities.

+++



4. **Architecture and Design**


A formal architecture or design document MUST exist, outlining key principles and documenting the design decisions that guided the implementation. It is RECOMMENDED that a "Security by Design" approach is followed to ensure security principles are integrated into every stage of the SDLC cycle.

A common practice is to maintain an [ARCHITECTURE.md](architecture) file within the repository.
This document SHOULD be released under a Creative Commons licence (or equivalent) and MUST be available without limitation to allow for public review and improvement.

+++


5. **Dependency Validation**


All dependencies SHOULD be validated against known security vulnerabilities.


+++


6. **Dependency Versioning**


The `project.toml` file MUST use exact version identifiers (e.g., `==1.2.3` rather than `>1.2`). This is a critical measure to prevent typosquatting and other supply-chain weaknesses. While [PEP 508](https://peps.python.org/pep-0508/ ) allows logical operators, for the purpose of this security standard, pinning to a specific version is required. Advantage is also that the Python part of the package is bit-for-bit reproducible. 


+++


7. **Reproducible Builds**


A package SHOULD be published using [Reproducible Builds](reproduciblebuilds). It is preferred to use a build tool for PyPI distribution that supports reproducible builds by default.


+++


8. **Principle of Least Privilege**


The program SHOULD require minimal privileges to execute. Administrative or high-privilege accounts MUST NOT be used if they could compromise the system. If specific authorizations are required, a separate service account MUST be created to facilitate clear security logging. The system documentation MUST clearly outline all required authorizations.


+++


9. **Defence in Depth**

The Defence in Depth principle MUST be practised across design, implementation, and testing. For instance, multiple SAST tools SHOULD be used for code validation to ensure comprehensive coverage.


+++


10. **SAST Scanning**


All Python source code MUST be validated using a trusted open-source SAST scanner, such as [Python Code Audit](https://github.com/nocomplexity/codeaudit). Where weaknesses are mitigated but still trigger a notification, they MUST be marked within the code with a clarifying comment.
