---
layout: post
title: Launching the Add Printer Wizard GUI as Admin
categories: [windows, printers]
---
I try to avoid using the Windows Add Printer Wizard when possible, but once in a blue moon I find that I need to run the GUI as admin and I do not want to log out the current user. We can do this by running the following command from an elevated command prompt:

`rundll32 printui.dll,PrintUIEntry /il`
