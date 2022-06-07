---
layout: post
title:  "How to list installed updates in Windows"
date:   2014-04-01 21:12:03 +0200
categories: 
---


Time to time you might need to list or export installed updates and hotfixes. Unfortunatelly even if you are able to lkst them in instaleld programs, you are not able to copy that list. But there are solutions.

In Windows 2003/XP  you have to use 3rd party software like [Windows Update List](http://www.nirsoft.net/utils/wul.html) by NirSoft.

In Windows 2008 and newer (works also for Windows 7 and probably Vista) it is much more easier, you can do it with:

`wmic qfe get /format:list >C:\installed_updates.txt`

Format can be:

- LIST  – tab delimited
- CSV – csv file
- HFORM/HTABLE – html
- RAWXML – xml

