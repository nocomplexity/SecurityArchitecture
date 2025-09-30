# Find vulnerabilities 

Periodic searching for new vulnerabilities for your used software and hardware is recommended. 

:::{caution} 
Relying solely on checks against known vulnerabilities (like those tracked by CVEs) provides a false sense of security!

The vast majority of vulnerabilities in software are never publicly reported. So recommended is e.g. to also use a **Static Application Security Testing (SAST)** tool. For Python programs, use the (FOSS) SAST tool [Python Code Audit](https://nocomplexity.com/codeaudit/).
:::

You SHOULD check vulnerabilities: 
* Regularly.
* When system is updated with new functionality.
* When significant security events in commonly used libraries are discovered. This to check if you are more vulnerable to.
* When infrastructure changes. E.g. new hardware or networking components.
* When evaluating new software. 



The Common Vulnerabilities and Exposures (CVE) process, which is the primary mechanism for reporting and tracking known flaws.

When a new CVE is out you are vulnerable. It does not matter if exploit code is already published on the Internet or not. Assume that Criminals are misusing the CVEs already.

A simple way to search for vulnerabilities is using `Search` option that the US National Vulnerability Database (NVD) offers. The NVD is a product of the NIST (National Institute of Standards and Technology).




````{admonition} Simple Vulnerabilities Search
:class: tip

Keep it simple: Use the direct search option of the NVD database.

```{button-link} https://nvd.nist.gov/vuln/search
:color: danger
Simple Search for vulnerabilities
```

````

:::{seealso} 
For a complete overview of all vulnerability databases, see the section:
[vulnerabilitydatabases](/references/vulnerabilitydatabases)
:::

