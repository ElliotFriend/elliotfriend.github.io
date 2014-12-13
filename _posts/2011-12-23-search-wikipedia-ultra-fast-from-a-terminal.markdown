---
layout: post
title: Search Wikipedia Ultra-Fast from a Terminal
author: elliotfriend
date: '2011-12-23 22:02:59 -0600'
categories: technology
id: 10
---
__I love Linux!__ There's no two ways about it! For the past few years,
I've become enamored with the open-source jewel that is Linux.

Lately, I've been going crazy with aliases. I've also been trying to make
my life easier with some simple Bash/Python scripts.

When my friends over at [Hak5](http://hak5.org) uploaded a HakTip about
searching Wikipedia from the terminal, I knew I had to alias/script it up!

Here's the script I put together:

{% highlight bash linenos %}
/bin/bash

# Store all arguments I provide as a string, SEARCH
SEARCH="$*"

# Replace any spaces with underscores, search wikipedia
dig +short txt ${SEARCH// /_}.wp.dg.cx
{% endhighlight %}

Combine that with an alias, like `alias wp='/home/elliot/scripts/digwp.sh'`,
and we get the following:

{% highlight shell-session %}
elliot@desktop ~ $ wp the tom green show
"The Tom Green Show is a North American television show which first aired
in September 1994 on Rogers Television 22, a community channel in Ottawa,
Ontario until 1996, and was later picked up by The Comedy Network in 1997.
(In 1996, Green also produced a p" "ilot episode for CBC Television,
although the CBC did not pick up the series.) http://a.vu/w:The_Tom_Green_Show"
{% endhighlight %}

I LOVE SHORTCUTS!!
