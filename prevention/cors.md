# CORS:Cross-origin resource sharing 

When dealing with internet and APIs you should familiar with Cross-origin resource sharing (CORS). 

This is a mechanism to safely allow a web page or API to access restricted resources from a server on a domain different from the domain that served the web page. 

This CORS specification is written for resource authors and user agents. 


Solid information on working of CORS and help for implementation can be found on the Mozilla website.

The main issue when applying CORS is misconfiguration. This happens a lot, mainly caused by implementation without a proper design or implementations that do not follow the design completely. Continuous testing when having configurations with CORS enabled is a must.



```{admonition} CORS rules are set by the server but enforced (voluntarily) in the client
:class: note, dropdown

* The server sets the rules: which domains can access their apis and endpoints plus various other rules.

*  The server *does not* enforce these rules. You can easily bypass CORS rules with postman, Curl, etc.

*   Chrome and other good browsers *will*  enforce CORS rules (which are set by the server).

*   The purpose of CORS is to protect front end clients (API customers) or ordinary end users (from cross site scripting, CSRF attacks, etc.) . CORS has nothing to do with protecting the server. If browsers did not enforce CORS then CORS would be pointless.

In short: The purpose of CORS is to protect clients, not servers. Rules that protect clients (or API consumers) are set by the server (and enforced voluntarily in the client. 

```



Resources for more information:
* [W3.org - Cross-Origin Resource Sharing](https://www.w3.org/TR/2020/SPSD-cors-20200602/)
* [Mozilla](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
* [Wikipedia](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing)
* [CORS protocol - Living Standard](https://fetch.spec.whatwg.org/ )
