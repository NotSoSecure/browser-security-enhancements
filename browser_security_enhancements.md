# Browser Security Enhancements

The browsers are currently implementing lots of changes day by day. We will be listing changes relevant to security enhancements which known browsers have implemented recently. To name a few, we will be discussing about the changes such as Tabnabbing protection, Referrer Leakage Preventions, HTTPS-Only mode, X-XSS-Protection and Cookie related security enhancement which can be used to prevent Client-Side vulnerabilities such as Cross-Site Scripting and Cross-Site Request Forgery. This list is aimed to be updated on regular intervals.

| Title | Description | Browser | Reference URLs| 
|---|---|---|---|
|Tabnabbing Protection|Reverse tabnabbing is an attack where an attacker can link a malicious page on the target application. The browsers recently added Tabnabbing protection and no longer allows access to the properties of "windows.opener". As browsers prevent Tabnabbing vulnerability and do not disclose "windows.opener" information to opener page, this shows a NULL response. We can say that the browsers eliminated the Tabnabbing vulnerability by securing opener information Additionally, if you want to opt out from Tabnabbing prevention, the web pages can use rel="opener".|Chrome 88+|[Anchor target=_blank implies rel=noopener by default](https://www.chromestatus.com/features/6140064063029248)|

