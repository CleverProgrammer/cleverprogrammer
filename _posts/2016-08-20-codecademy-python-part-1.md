---
layout: post
title: "Codecademy Python: Part 1"
subtitle: Variables, whitespace, comments, math operations, modulo, indexing, and much more!
categories: [programming, codecademy, python, tutorial]
tags: [programming, computer science, coding, python, codecademy, tutorial, walkthrough, part1]
published: True
permalink: codecademy-python-tutorial-1
author: Rafeh Qazi
comments: true
---

# Codecademy Python: Part 1
This is part 1 of the Codecademy Python Walkthrough Tutorial. It covers topics like variables, whitespace, comments, math operations, modulo, string formatting, indexing, functions, methods, and string concatenation.
<iframe width="560" height="315" src="https://www.youtube.com/embed/2dmBp5RydwE" frameborder="0" allowfullscreen></iframe>

### Rafeh Qazi

Hey guys, how are you doing? Today I'm going to take on an interesting challenge which is going to be I'm going to go through the entire Codecademy class and finish it as fast as I can. And along the way my goal is to be able to help you, give you some kind of intuition. For most of you that are stuck, I want to help you get unstuck and think about code in a different way, I hope. I hope that this video helps you and helps you solve those annoying, frustrating problems. I remember when I was going through this I didn't have any help and I would quit for weeks at a time because I did not know where to go. Even the forums didn't help me. So that's my main point, to help everybody else out there. So we're going to be taking the Codecademy course here. We're going to take it in the language called Python. There are tons of students enrolled here, 2.5 million, it's a fairly long course, and the level required is beginner. 
Unit 1 is Syntax, Tip Calculator. Unit 2 talks about Strings, Date & Time. As we go on down we go into more and more useful and advanced things. Conditional and Controlled Flow is going to be fun. Functions. Dictionaries. And pretty much all of the stuff here-Battleships is going to be a lot of fun. Feel free to use this video to help you if you get stuck, or for entertainment, you can just sit through and watch along how I tackle these problems. 
So the first one is Python is an easy programming language. You can use it to create web apps, games, even a search engine. Ready to learn Python? Click save and submit. The first problem is already done. All I have to do is hit "save" and submit code. Okay, streak of 1. 
Start next lesson. Creating web apps, games and search engines all involve storing and working with different types of data. You do so using variables. Variables store a piece of data and gives it a name. For example, spam=5. So basically here they're teaching you how to store a variable name (my_variable) and value (10). What I need to do, they gave me the steps right over here. So I'm going to say 

1.	`my_variable=10`

And that's all I need to do here. That was very simple.  Next set the variables to the values listed in the instructions. A=true, b=false, and we're done. They are talking about Booleans here. Boolean values are true and false, like a light switch, BOOM one is on, one is off. Then they want us to set my_int=7, my_flow=1.23 and my_bool=true. 
Now. You have been reassigned. Here we're going to reassign values. Initially my_int was 7, and I'm going to change my_int to 3, and that's it for this one. (Types my_int=3 on designated line.) Sweet.
Now we get into functions and functions are fairly cool. This code is poorly formatted because every time you write def you've got to indent 4 spaces, 4 or more spaces, after you write the colon. This is called a function. We wrote a function called spam and what it does it make x=12 and then it returns eggs. So it sends these instructions. They're part of the overall function, and need to be indented underneath the function. Let's go ahead and indent this, and hit submit. That's good. 

```1.	def spam():
2.	eggs = 12
3.	return eggs
4.	      
5.	Print spam()```

This gives indentation error. Whitespace is important in Python and we need to indent all of these otherwise we'll get errors. A window in the right top of the page is called interpretor. The interpretor runs your code line by line and checks for any errors. In this example they make a variable called cats and assign it the value 3. We're supposed to create a variable called spam and set it to true and create a variable called eggs and assign it the value false. 
```1.	Spam=true
2.	Eggs=false```

Single line comments-comments are things that are ignored in Python. They are things that are ignored in any programming language. The point of a comment is to tell a program "don't read this". It's reading everything else but don't read anything that has this special symbol next to it-it's a comment, it's only meant to be read by a human being, and the computer has nothing to do with it. If I said 5+5 the computer might give me back a 10, but if I put this as a comment the computer's not going to give me back anything. If I write # rd{}x0 the computer will just ignore it. It reads it as a comment. That's the point behind the hashtag symbol (number symbol #) or a comment. Write a comment on line one, make sure it starts with #. So we can say anything we want. (He writes # hi I'm a very clever programmer.) 
Multi-line comments, the point is you can write multiple lines without having to put # at the beginning of each one. You put """ (3 sets of quotes) before and after the comment""" just like that. Everything inside the quotes, no matter how many lines it takes up, is a comment. You may not understand documentation, because you may be a beginner, but you can use comments for documentation, to tell someone else what you're doing in your program.
Now let's do some math. In programming languages you can do a lot of math. It's fun. If I opened up my terminal, I can open up Python and I can do 5+5 or 10+10 or 10 x 20 (which is written 10*20), then the answer appears on the next line line this:
```>>> 5 + 5
10
Or
>>>10 * 20
200```

So let's do addition. Instructions: Set the variable count_to equal to two big numbers. 
>>> count_to = 546 + 726
Let's look at exponentiation. You use the up arrow symbol to indicate an exponent. 4^2 means 4 to the second power which is 4 squared, or 16. 3^3 is 3 to the third power which is 3 x 3 x 3 or 27. You can also write this 3 = 3 **3 or 16= 4**2.
Instructions: Set eggs equal to 100 using exponentiation: 
I'm going to do it like this: 100 is 10 squared so I write
Eggs = 10**2
You could also say 
Eggs = 5**2 * 4  (proper order is to do the exponent first, or 5 x 5 =25, then do the multiplication, or 25 x 4=100)
Next is the modulo operator. It's basically the remainder from a division, and % is the symbol for the modulo operation, so if you have 10 divided by 2, doesn't 2 go into 10 evenly, with no remainder? Then modulo will be 0. This would be written like:
10 % 2
0
Another example:
10 % 3
1
(the computer comes up with 1 because it is the remainder of 10 divided by 3)
And note the difference between division and looking for remainder:
11/2
5.5
11%2
1

Now, bringing it all together. Variables are like x=5, y=2; they store values. In data types, you have numbers, strings, a list, a dictionary. If you don't know what a dictionary or list is, ignore that for now. Just remember 5 and hello are different kinds of data types. And if I say true, that's a different type, too – the word for true and false is Boolean, remember? White space is what separates the statements. If I say x=5 and y=4, those statements have to be separated. You can't do them on the same line, you have to give it some white space, and white space is just blank. In Python white space is very, very important; in other programming languages, it may not be. Comments: How can I make a line a comment? Add a hashtag sign (number sign) in front of it. My code will run and ignore the comment. Arithmetic operations-pretty straightforward. Addition and subtraction, multiplication, division, exponentiation, and then the module operation. 
Instruction: Write a single line comment on line 1. Set the variable monty equal to true. Set another variable python equal to 1.234. Set a third variable monty_python equal to python squared.

1.	   #Hello youtube audience
2.	    monty=true
3.	    python=1.234
4.	    Monty_python = python **2

Next is Tip Calculator. Start lesson. That's what I'm here for. We're applying the concepts from the previous section to a real world example. Now we're getting to the fun part of coding. You've finished eating a meal, and want to apply the tip to the whole cost including tax. We're given these numbers:
Cost of meal $44.50; Restaurant tax is 6.75%; Tip is 15%.
First, declare the variable meal and assign it the value of 44.50:
Meal = 44.50    You always see me writing spaces before and after the signs (like the = in this example).             That is considered good code, where the spaces help provide readability. This is the accepted standard       for doing this.
Tax is equal to 6.75%, which is 6.75/100
Tax = .0675
Tip is 15% or 15/100.0. I must put the decimal in order to get an exact number. Without it, I get only the integer, which for 15/100 is 0. 
Tip = 0.15
Assign meal to the value of itself plus tax: 
Meal = meal + meal * tax   This gives you a further amount for the meal by adding on the tax.
Assign the variable total to the sum
Total = meal + meal* tip      This takes into account the total you paid for meal and tax, plus the amount you are paying in tip, and gives you the grand total of your spending for the entire meal. 

Next we have strings and console output. I'm going to create a variable called Brian and assign it the value hello life. 
Brian = "hello life!"   hello life! Is a string. I can put anything I want in there. It's completely arbitrary. Hello life doesn't have any value. It isn't a variable. However, Brian is a variable. If you typed in Brian, you'd get back Hello life! Now some practice with strings.
Set caesar to equal "Graham", praline is equal to "John" and viking is equal to "Teresa"
Caesar = "Graham"
'Praline = "John"
Viking = "Teresa"
Next, the string below is broken. Fix it using the escape backslash! First, the broken string:
'This isn't flying, this is falling with style!'
The quotes at each end mean you're trying to put this entire thing into a string. The main problem is it thinks the apostrophe in isn't is ending the string. The solution they want here is to use the escape backslash, so you put it right in front of the apostrophe and basically it says don't think of this as a quote. 
'This isn\'t flying, this is falling with style!' 

Next section is Access by Index
Characters in a string can be referred to by their index number, by the order they appear in the string. For example, the word P Y T H O N has six characters, and they are numbered beginning with zero (0). If you want to get the t you can type "python"[2]. Always remember, start counting with zero! 
To get the fifth letter in MONTY you need index number 4. To refer to it, you write
Fifth_letter = "MONTY"[4]    
I can change from upper to lower case by writing
"Monty".lower
Monty
To make upper case from lower case I write
"monty".upper
MONTY

Now, you can use a number as a string or part of a string. It will be treated as a letter and only string functions can be performed with it. It cannot be added or multiplied or any arithmetic functions performed on it. Look at this:
>>> str(5)
'5' 
>>> "5" + "5"         (Putting together two strings, not adding)
55
>>> 5 + 5              (Now you are adding two numbers, no quotes, so not strings)
10


Instruction: On line 1 create a variable named parrot and set it to the string "Norwegian Blue".
1     parrot = "Norwegian Blue"
2     print (len(parrot))
3     14 is the length of the string, so it returns 14
You can do lower and upper on this string, with the expected results.

Note: methods that use dot notation only work with strings. On the other hand, len() and str() can work on other data types.
Ministry = "The Ministry of Silly Walks"
Print len(ministry)         
27

When you do the plus sign on strings it just concatenates, meaning it combines the strings to make one long string.
Instruction: Print the concatenation of "Spam and eggs"
Print ("Spam " + "and " + "eggs" )        Notice I put a space behind the word spam and the word and so that they are printed that way. 
Spam and eggs

## End of Tutorial #1


## ABOUT PYTHON CODECADEMY SERIES
This is meant to guide you through the codecademy python part and it also to help you get a much better understanding of the code that you to write according to the instructions on CodeCademy.com. This will help you understand many programming concepts and the concepts that are tricky, I open up an interactive prompt and I will also ask you questions along the way to keep it more interactive for you. I believe teaching only works when you actively engage. 

The target audience are beginners or developers looking to pick up Python. I also emphasize the importance of writing good code and I go through the first part really fast.

I will literally be going through every single thing and breaking it down for you so there is nothing for you that would be scary. You can watch me do it and you can simply follow along you will learn ALL the basics. I swear I wish something like this was out there when I started learning because everyone else explains things in such a complicated way and makes it so boring! I honestly think programming is based upon exploration and creativity rather than some mathematical/logical genius frame of mind! I spent a lot of hard work in making this so I hope you guys enjoy and learn something out of it while having fun! This is targeted towards beginners, for developers looking to learn python, or for individuals looking for a refresher on basics in computer programming!!