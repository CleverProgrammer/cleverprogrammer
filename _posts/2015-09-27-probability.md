---
layout: post
title: Know Your Probability Basics
subtitle: "How can we use probability to better understand the world around us?"
categories: [Coursera]
tags: [Probability]
published: True
permalink: probability
author:    "Rafeh Qazi"
header-img: "img/iphone-passcode2.jpg"
comments: true
---
#The Joys of Probability
<img src="{{ "/img/iphone-passcode.jpg" | prepend: site.baseurl }}" alt="image">

1. How many possible 4-digit passcodes can you have on your iPhone 6? (Enumerations &amp; Permumations &amp; Combinatorics)<br><br>
2. How many centuries will it take to break a password with an entropy level of 77? (Security)<br><br>
3. If you got heads on the first flip... What is the probability you will get heads again? (Independent vs Dependent variables)<br><br>
These are some of the many questions that probability helps us answer.

## So... Let's get started!
So let's start off with the iPhone 6 passcode question. How many possible ways of rearranging the 4 digit passcodes are there?
To answer that, we need to understand something important about probability. If we have some random **sequence** of some length (think of the 4 digit passcode) and we have a set of **outcomes** (think 0,1,2,3,4,5,6,7,8,9) we can use this information alone to get our answer. So let's start off with an easy example: If we were allowed to make a passcode with length of 1 (1 digit passcode instead of a 4 digit passcode), our passcode would only have 10 possible ways of rearranging it <br>

<h2><font color="red">Total enumerations with One-Digit Passcode</font></h2>

|0| |1| |2| |3| |4| |5| |6| |7| |8| |9|

But now if we were allowed to make our passcode with length 2 (2 digit passcode) we would now have 100 possible ways of arranging the 2 digit passcodes! This means that if someone was given 100 tries and they tried every single possiblity, they would be able to break your passcode! Here's a cute little python list comprehension to generate all the possible enumerations:

{%highlight python3%}
[ (row, col) for row in range(10) for col in range(10) ]
{%endhighlight%}

<h2><font color="red">Total enumerations with Two-Digit Passcode</font></h2>

|00| |01| |02| |03| |04| |05| |06| |07| |08| |09|
|10| |11| |12| |13| |14| |15| |16| |17| |18| |19|
|20| |21| |22| |23| |24| |25| |26| |27| |28| |29|
|30| |31| |32| |33| |34| |35| |36| |37| |38| |39|

If we were to continue this pattern at the end it would look like:
 <br>

|90| |91| |92| |93| |94| |95| |96| |97| |98| |99|

If we were to count all of these out, you would find that there are a 100 different **enumerations** of a passcode with a sequence of 2 numbers and an outcome of 10 numbers (0-9 possible numbers)! Pretty cool huh?! But, what if we wanted to generalize it in a way where we could find all the enumerations of any sequence with any number of outcomes? Here is a pattern to keep in mind: `outcomes` will be multipled by `outcomes` the same number of times as the length of the `sequence`.<br>
In short: `outcomes`^`sequence length` will give you all the possible enumerations<br>

| Outcomes (0-9) | Sequence Length (1-4) | Calculation | **Total Enumerations** |
|----------|:---------------------------:|:--------------:|---------------------:|
|    10    |         1       | 10^1|  10     |
|    10    |         2       | 10^2|  100    |
|    10    |         3       | 10^3|  1,000  |
|    10    |         4       | 10^4|  10,000 |

<img src="http://i.imgur.com/uujWjyz.jpg" alt="die enumerations">

Now 10,000 possible enumerations might seem like a lot and it might seem like the phone would be safe, however, that is simply not true. 10,000 enumerations are very small and powerful password decryption tools can guess 100's of millions of possible enumerations per second. The thing that keeps you safe is how the iPhone will lock itself for increasing number of seconds per failed attempt. <br>

So to answer your question of how many possible enumerations of four-digit passcodes for your iPhone there are, with a bang: <br>
<h2><font color="red">There Are 10,000 Possible enumerations for Your iPhone 6 Four-Digit Passcode</font></h2>
<img src="http://i.imgur.com/0k9qUTw.jpg" alt="iPhone 6 Pass Codes">

#Now let's introduce a new idea.
So far we have discussed `enumerations`. Now let's discuss `permutations` and `combinations`.<br>
Let `m` = outcomes <br>
Let `n` = sequence <br>

| Permutations | Enumerations | Combinations |
|:----------:|:--------------:|:------------:|
| `m!/(m-n)!`|     `m^n`      | `m!/(m-n)!n!`|


Programming trick in python to generate `permutations` and `combinations` less expensively:
{%highlight python3%}
num_permutations = 1
for number in range(m, m-n, -1):
  num_permutations *= number
print(num_permutations)  # Permutations

print(num_permutations / factorial(n))  # Combinations
{%endhighlight%}

###Now let's look at some tangible examples: <br>
Say we are playing a lottery and we can draw 6 numbers from a range 0...59. Here is how we will be able to figure out all the possible `enumerations`, `permutations`, and `combinations`: <br>

{%highlight python3%}
num_permutations = 1
for number in range(59, 59-6, -1):
  num_permutations *= number
print(num_permutations)  # Permutations  => 32,441,381,270

print(num_permutations / factorial(6))  # Combinations  ==> 45,057,474
print(59**6)  # Enumerations  ==> 42,180,533,641
{%endhighlight%} 
