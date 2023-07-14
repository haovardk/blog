---
layout: post
title: How do you handle Azure Enterprise Application and API permission?
subtitle: If "I let my users consent to whatever the appliations ask for" is your strategy - please read on
tags: [Microsoft Azure, Security]
comments: true
---
Vasil Michev wrote a good article back in 2021 about "Inventorying Permissions to Azure AD Apps".
The link and procedure on how to check access: https://practical365.com/inventorying-azure-ad-apps-and-their-permissions/
The Powershell script that is beeing used can be found here: https://github.com/michevnew/PowerShell/blob/master/app_Permissions_inventory_GraphAPI.ps1

The article still holds water today. I see far to many organization that allows the users to consent to any requests that third party applications asks for. 
Do you want a third-party application to get access to all files that the signed in user can(Files.ReadWrite), list all mail and calendar events that the user have access to(Calendars.ReadWrite)?
I hope that the answer is no. 

Take a look on how Microsoft recommends you to configure consent: https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?pivots=portal