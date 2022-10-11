---
layout: post
title: Multifactor authentication and break the glass account
subtitle: There is a reason why you should have it
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---


Multifactor authentication is a hot topic. And so is the increase in securing organization accounts.
Microsoft are providing the ability to utilize SMS, email, phone call or app authentication as a second factor in secure logins.

Follow this link to how to “Set up multi-factor authentication”:
https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide

But what do you do if these services are not available? 
It could be a telecom outage where you do not have a signal to receive phone call or SMS. 
Or it could be that the Microsoft 365(and Azure) platform have degraded service so that you cannot use email or app authentication.

And you need to login to do some changes. Now. Immediately. Asap.

This is where break the glass (BTG) accounts come into place. 
Microsoft recommends having at least one emergency account. This account should not be personal and must be excluded from MFA.

It should have a complex password, and the usage must be extra monitored.

Microsoft have created a good guide for this: 
https://docs.microsoft.com/en-us/azure/active-directory/roles/security-emergency-access#monitor-sign-in-and-audit-logs

This account must also be excluded from the MFA registration policy in Identity Protection:
![Bobst](https://i.imgur.com/fj90szT.png “IdentityProtection”)