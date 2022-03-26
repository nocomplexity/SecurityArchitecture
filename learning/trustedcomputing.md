# Secure Computing

Secure computing environments aim to created better confidential computing environments. Trusted Execution Environment (TEE) technologies exist on multiple levels (hardware, software, CPU). Open Trusted Environments can provide real improved trust and remove risks that can not be fully eliminated on traditional systems.

## Confidential Computing Consortium Projects

The [Confidential Computing Consortium](https://confidentialcomputing.io/) is a community focused on projects securing data in use and accelerating the adoption of confidential computing through open collaboration.

[The projects list](https://confidentialcomputing.io/projects/)


## Enarx

Application deployment system enabling applications to run within Trusted Execution Environments (TEEs).
Enarx is a framework for running applications in TEE instances – which we refer to as “Keeps”–without the need to trust lots of dependencies, without the need to rewrite the application, and without the need to implement attestation separately.

Enarx aims to minimize the trust relationships required when executing applications, meaning that the only components which need to be trusted are: the CPU and associated firmware, the workload itself, and the Enarx middleware, which is fully open source and auditable. Applications run without any of the layers in the stack (e.g. hypervisor, kernel, user-space) being able to look into or alter the Keep or its contents.

[http://enarx.io](http://enarx.io)

## SeL4

seL4 is a high-assurance, high-performance operating system microkernel. It is unique because of its comprehensive formal verification, without compromising performance. It is meant to be used as a trustworthy foundation for building safety- and security-critical systems. It is available as open source on GitHub and supported by the seL4 Foundation. 

Github repository: [https://github.com/seL4/](https://github.com/seL4/)
Landing page: [https://sel4.systems/](https://sel4.systems/)