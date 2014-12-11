---
layout: post
title: Find Directory and File Size in a Terminal
author: elliotfriend
date: '2013-02-19 16:40:32 -0600'
categories: technology
header-img: "img/post-bg-01.jpg"
subtitle: This is something that should be in your sysadmin toolbelt!
---
Here's a really handy command that I tend to forget exists.

If you're running out of disk space, it can be really hard to track down
a runaway file. Here's a way you can get some more information:

{% highlight bash %}
du -hs /path/to/directory/or/file
{% endhighlight %}

This helped me figure out once where **114GB** log file was taking up
all my space! Super handy!

I will note that if you are trying to find the size of all files or
directories in a given directory, use the asterisk to target them all:

{% highlight bash %}
du -hs /home/elliot/*
{% endhighlight %}
