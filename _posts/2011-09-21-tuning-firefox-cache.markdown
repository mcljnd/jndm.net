---
layout: post
title:  "Tuning Firefox: cache"
date:   2011-09-21 21:12:03 +0200
categories: 
permalink: /2011-09-21-tuning-firefox-cache/
---

If you have plenty of RAM and do no want Firefox to save temporary files to disk (for example because you have SSD and want to limit number of disk writes) you can move Firefox cache to RAM.

There is no way how to do it in gui, so you need to use favorite *about:config*.  Search for parameter *browser.cache.disk.enable* and set that to **false**. Now disk cache is disabled. Then search for *browser.cache.memory.enable* and set that as **true** – it will enable cache in RAM (it is set to true already sometimes).

If you want to set how much RAM you will dedicate to cache, search for *browser.cache.memory.capacity* and as value set desired cache size in kilobytes.

Moving cache to RAM is good idea only if you have quick internet connection as cache is wiped out on every restart and all pictures, scripts etc. are downloaded again after restart.
