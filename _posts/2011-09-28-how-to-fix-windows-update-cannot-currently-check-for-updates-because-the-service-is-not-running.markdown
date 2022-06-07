---
layout: post
title:  "How to fix “Windows Update cannot currently check for updates, because the service is not running”"
date:   2011-09-28 21:12:03 +0200
categories: 
---
Sometimes you can get in situation that Windows Update is not working and you are receiving error

> “Windows Update cannot currently check for updates, because the service is not running. You may need to restart your computer”.

It can be caused by corrupted data for Windows update. If this is your case fix could be easy.

- go to services and stop Windows update service
- locate C:\Windows\SoftwareDistribution\ folder and delete all its content
- start Windows update service
- check for updates
