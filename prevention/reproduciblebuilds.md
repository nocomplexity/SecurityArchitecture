# Reproducible builds

When using FOSS software you have the advantage to inspect the source code on malicious flaws. However almost all software is distributed to end users as pre-compiled binaries. This creates a problem: How do you know if the software is not injected with malicious code?

Compiling the software yourself is not enough to be sure that no flaws have been introduced.

```{attention} 
You **should** check if your software has a reproducible build.
```


From a security perspective it is desirable that building a binary the same source code with the same set of tools is reproducible. So that the output is always exactly the same. This makes it possible to verify that the build infrastructure for a binary distribution or embedded system has not been subverted. 


```{tip} Simple security tip 
For good security you should check if your software has a reproducible build. So validate that the output of your software build matches that of the original build.
```

Whilst anyone may inspect the source code of free and open source software for malicious flaws, most software is distributed pre-compiled with no method to confirm whether your received software package matches the software that it is supposed to be.


## What is a reproducible build?
A build is reproducible if given the same source code, build environment and build instructions, any party can recreate bit-by-bit identical copies of all specified artifacts.

So a reproducible build is, an approach to determine whether generated binaries correspond
with their original source code. 


The motivation behind the Reproducible Builds project is to allow verification that no vulnerabilities or backdoors have been introduced during the software compilation process. 

For all software and software build systems in use it is crucial to notice if a developer or build system has been compromised. 

Creating a reproducible build requires some steps. But if you produce software you should do these steps anyway to make sure your software build process is secure. 

Steps to create a reproducible build:
1. Make your build system entirely deterministic: transforming a given source must always create the same result. For example, the current date and time must not be recorded and output always has to be written in the same order.
2. The set of tools used to perform the build and more generally the build environment should either be recorded or pre-defined.



More information: [https://reproducible-builds.org/](https://reproducible-builds.org/)

A nice introduction paper covering the reproducible build project can be found [here](https://arxiv.org/pdf/2104.06020.pdf).

*(Attribution: Some text in this section is used from https://reproducible-builds.org/, licence cc-by-sa.)*

