---
layout: post
title:  "How to update Windows defender automatically"
date:   2013-04-16 21:12:03 +0200
categories: 
---

Windows 8 brings not only Metro interface and strange Start menu but also Windows Defender instead of Microsoft Security Essentials. Windows Defender is missing some features MSSE has. One of those changes is that updates for virus and spyware definitions are installed by Windows Update.

In case your setting are “notify but not install automatically” you are asked nearly every day for manual update. My guess is that Microsoft want to force people to use automatic updates.

Fortunatelly Windows defender has also command line utility, so you can easily update definitions from command line:
{% highlight console %}
C:\"Program Files"\"Windows Defender"\MpCmdRun.exe
{% endhighlight %}

will show you options and examples. For update from command line is important this one:
{% highlight console %}
C:\"Program Files"\"Windows Defender"\MpCmdRun.exe -SignatureUpdate
{% endhighlight %}

Easiest way is to create scheduled task which will check for new defitions lets say once a day and number of requests to install updates will be lowered significantly.
