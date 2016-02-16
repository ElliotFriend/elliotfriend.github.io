---
layout: post
title: Fibonacci Sequence in Python
author: elliotfriend
date: '2014-03-09 00:55:38 -0600'
categories: technology
img-name: "golden-spiral.jpg"
subtitle: Who knew it could be so easy and gratifying?
seq: 15
comments: true
---
In case anyone ever wanted to know how to run the Fibonacci Sequence in
Python, here's how I did it:

{% highlight python linenos %}
/usr/bin/env python

import sys

f_seq = [ 0, 1 ]
while len(f_seq) <= int(sys.argv[1]):
    f_seq.append(f_seq[-1] + f_seq[-2])

print f_seq
{% endhighlight %}

Now, all you have to do is run `fibonacci.py 20`, and it will give you
all the numbers through F20 (starting at zero).

Update: [I put this up on Github](https://github.com/ElliotFriend/bin/blob/master/fibonacci.py)
, and have made a couple changes since I
initially wrote it.

Photo by [IPBrian](https://flic.kr/p/aLKwzT)
