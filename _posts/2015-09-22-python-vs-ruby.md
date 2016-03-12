---
layout: post
title: Python Vs. Ruby
subtitle: Differences between Python and Ruby
categories: []
tags: []
published: False

---
#For loops

<font color="blue">Python</font>
{%highlight python3%}
for i in range(5):
 print(i)
#==> 0
#==> 1
#==> 2
#==> 3
#==> 4
{%endhighlight%}

<font color="red">Ruby</font>
{%highlight ruby%}
(0..4).each do |i| puts i end
#OR
(0..4).each{|i| puts i}
#OR
(0...5).each{|i| puts i}
#==> 0
#==> 1
#==> 2
#==> 3
#==> 4
{%endhighlight%}