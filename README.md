# Tracking Browser Security Enhancements

### Introduction
Our lives have been slowly moving from desktop applications to browser-based applications and browsers have become an integral part of our life. Current top browsers have a special focus on security and have been working on many major security projects to kill bug classes. Some are ambitious projects, some are smaller tweaks. Some continue to become the core of the browser, some projects get shelved or discarded.

With processing powers shifting to client-side, the browsers have focused extensively on the client-side vulnerabilities and on providing a safe space for the applications and its users. Largely the focus has been centered around killing bug classes such as Cross-Site Scripting and Cross-Site Request Forgery, as well as enhancing privacy for the end users. Some of the recent changes implemented by browsers are HTTPS-Only mode, Cookie related security, Tabnabbing protection, Referrer Leakage Preventions, and X-XSS-Protection to name a few.

This brings in an interesting situation for information security professionals as our recommendations and risk ratings can get affected by these changes. We have been trying to keep a tab on these changes internally and we realised that it makes sense to make this information public.

### What is the Browser Security Enhancements Tracker Project?
At NotSoSecure we have been internally tracking these changes as this eventually affects how we give out recommendations to our customers. We decided to make these details public in an effort to make more people aware about these, as well as enrich the content via public contributions. 

With this aim in mind we are launching the Browser Security Enhancement Tracker Project today. We aim to keep a track on major security related enhancements or downgrades implemented by browsers. We have a list of all entries as well as a dedicated page talking about specific entries. 

##### To access the project website, [Click Here](https://notsosecure.github.io/browser-security-enhancements/).

### Why Do Security Professionals or Web developers Need to Look at the Recent Browser Changes?
These browser changes are often implemented by means of header or default attribute changes, which changes the behavior of vulnerabilities or completely removes them, however, it can also affect the working of an application. Such changes make the browsers more secure but as security practitioners, we must be aware of the changes implemented by the browser. For example, many browsers have recently implemented Tabnabbing prevention by restricting the access to the opener properties. If the opener properties are not shared with the opener page, it would not allow access to the resources. Optionally, if you do want your page to have access to opener properties that can be facilitated by using rel=”opener”. This and many more such entries can be added in the tracker.

### Can Anyone Update the Browser Security Enhancements Tracker?
Yes, we encourage everyone to help us make this list better. Each contributor name will be listed in the contributors section on [About](https://notsosecure.github.io/browser-security-enhancements/about/) page.

Contributors can contribute by creating a new post or modifying the existing one. To contribute a new post, you can follow the next step:
1. Add the new file at "https://github.com/NotSoSecure/browser-security-enhancements/tree/main/_posts". Filename should be "YYYY-MM-DD-{Title/Vulnerability/Update}.markdown". 
2. Create a file using the template given after this listing. 
3. Push it on GitHub, we will validate this and publish it.

##### Template for adding a new post:
```
---
layout: post
title:  "{Title/Vulnerability/SecuirtyUpdate}"
date:   YYYY-MM-DD HH:MM:SS +0530
categories: Security Updates
published: true 
description: {Give a short description which will be displayed on the listing page, https://notsosecure.github.io/browser-security-enhancements/}
browsers: {Browser versions from which version the changes have been implemeneted, like Chrome X+ FireFox X+}
---

## Description 
{Description here, markdown is preferable - Example URL: https://notsosecure.github.io/browser-security-enhancements/}

## Browser(s) 
{Browser versions from which version the changes have been implemeneted, like Chrome X+ FireFox X+}
* Chrome X+
* FireFox X+ 

## Reference(s)
* [Title1](Link1)
* [Title2](Link2)
```
