---
layout: post
title:  "zsh – how to reload .zshrc"
date:   2020-02-10 21:12:03 +0200
categories:
permalink: /2020-02-10-zsh-how-to-reload-zshrc/ 
---
After editing your .zshrc you may need to reload it so changes are applied. Its quite easy:

{% highlight bash %}
jndm@Macbook ~ % source ~/.zshrc
{% endhighlight %}

or shorter:

{% highlight bash %}
jndm@Macbook ~ % . ~/.zshrc
{% endhighlight %}