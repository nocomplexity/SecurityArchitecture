# Simple Solutions



```{admonition} How to mitigate DDoS attacks - never simple..
:class: tip, dropdown
A Denial of Service (DoS) attack is an attempt to affect the availability of a targeted system. Typically, attackers generate large volumes of packets or requests ultimately overwhelming the target system. In case of a Distributed Denial of Service (DDoS) attack the attacker often uses multiple compromised sources to generate the attack. Like cloud services. Also a DDoS attack can be used as a distraction to get unprivileged access. 

DDoS attacks are most common at the Network (layer 3), Transport (Layer 4), Presentation (Layer 6) and Application (Layer 7) Layers.

Simple rules for mitigating DDOS attacks:
* Design a good but simple architecture
* Create a static version of your site to be able to inform customers
* Have a response plan
* Have different mitigation scenarios in place
* Make sure to have a direct phone number of a real network security expert that can and will help you! (Without ripping you off)

[{bdg-primary}`Read this blog for more in depth information`](https://nocomplexity.com/one-more-time/)
```

## Prevention


```{admonition} Create a Security Architecture
:class: tip, dropdown

So follow these simple steps:
* Do a risk analysis.
* Develop a security architecture based on your risk profile.
* Always consider real distributed solutions where your security concerns are to spread across several nodes to reduce the impact of a single breach. E.g. spread data and secrets across several independent nodes to be more resilient.  
* Develop a thread analyse and improve your architecture.



```

## Protection


```{admonition} Implement simple measurements that really help!
:class: tip, dropdown

Most security protection measurements are very simple and extremely effective.

So just do:
* Developing awareness within your company and following awareness trainings a continuous process! 
* Always implement virus protection on MS Windows based platforms.
* Always implement network segmentation.
* Always implement some simple firewall rules. 


```

## Detection

```{admonition} Implement simple measurements that really help!
:class: tip, dropdown

Implement some simple but good detection measurements to detect security breaches. Else:everything you do is useless.

So just do:
* Use audit logging on file systems. Simple is: Use the audit capabilities that are delivered on your operating system. E.g. The FreeBSD audit system for determining read,write,changes on systems is simple but very effective. So use this [FreeBSD Audit Handbook](https://docs.freebsd.org/en/books/handbook/audit/ ).
* Use the default detection system to log and audit all successful and unsuccessful login attempts on your network.


```

## Respond

```{admonition} Implement some simple procedures to respond to security incidents.
:class: tip, dropdown

Do not reinvent the wheel. For every simple or complex security incident a good procedure is already invented. 

So just do:
* Use and reuse existing security incident procedures. 

A good collection can be found here [link]


```

## Recover

```{admonition} Make sure you have a recovery plan.
:class: tip, dropdown

Do not reinvent the wheel. A good recovery plan is simple: 
* Make backups and test recovery procedures.

Automate making the backups. But make sure that recovery is always manually verified.
Test for disasters. So never ever assume that your backups can not be compromised or stolen.


```