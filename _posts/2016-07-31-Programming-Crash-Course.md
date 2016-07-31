---
layout: post
title: Programming crash course
---

Coding is super fun, and can be very rewarding, but in order to be able 
to complete any projects, we first have to have a basic understanding of 
programing constructs.

Programming languages are designed as a bridge for humans to be able to 
give computer a series of instructions to follow to complete a task. 
They have evolved from punch cards, to machine language, to systems 
programming languages, and finally high level object oriented and 
functional programming languages. Language evolution is driven by our 
desire to get more done in less time and with less effort.

Ultimately, whatever language we choose to code in, the most important 
part is how easily we can get our idea from the inside of our heads to 
running on a computer.

# Language Similarities

Almost all programming languages share a few common features:

- They provide a way to store the value of an intermediate calculation. 
These storage locations are called variables.
- They provide a way to encapsulate blocks of code into reusable pieces. 
The most primitive of these is normally in the form of a function.
- They provide a way to run a block of code N times. This functionality 
is provided either as a loop construct or a way for a function to call 
itself the requisite number of times (this is called recursion). We’ll 
cover for and while loops.

Understanding these basic similarities is essential to writing any 
computer program. For the remainder of this document, we’ll provide some 
examples of how these features are used to build a functional computer 
program.

# Getting started

At dinner and code, we concentrate on two languages to start off new 
programmers with. Python, and/or javascript.

### Python
A modern, interactive, object oriented programming language. Its clear 
syntax and extensive libraries make it a great choice for beginners that 
want to learn to code without having to write absolutely everything 
themselves.

### Javascript
A prototype based programming language. Javascript has quickly become a 
requirement for any serious front end web development work. Its ubiquity 
makes it a great language to learn to accomplish a large variety of 
projects.

No matter which of these languages you choose to begin learning about, 
we’ll provide examples in this guide to explain the basic concepts.

### Getting started in Python

You’ll need to download the python programming language from the 
internet to get started in python programming. To do this, head over to 
https://www.python.org/downloads/ and choose the latest version of 
Python 3.0 that is available on the page. Make sure you download the 
version for your operating system. Once python is installed, you can 
click on the IDLE editor that comes with the package and start typing 
in code right away.

### Getting started in Javascript
The easiest way to get started in Javascript is simply to navigate to 
jsfiddle.net where you’ll be able to type in HTML, JS, and CSS and see 
the results of what you’re doing right away.

---

# Variables
Variables allow you to save the result of some work that has been done 
for later use. Let’s say for example that you’re writing a program that 
adds two numbers together and do something later with the result. We can 
use variables to store the result and print it out. 

### Python Example
Open up the IDLE editor and type in a = 5 and then press enter. The 
screen should look something like this below.

```
Python 3.5.1 (v3.5.1:37a07cee5969, Dec  6 2015, 01:54:25) [MSC v.1900 64 bit (AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> a = 5
>>> 
```

This has assigned the value of 5 to the variable _a_. We can now use _a_ 
later on in the program whenever we need the value again. We can see 
this by telling python to print out the value of a by typing _print(a)_ 
as shown below.

```
Python 3.5.1 (v3.5.1:37a07cee5969, Dec  6 2015, 01:54:25) [MSC v.1900 64 bit (AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> a = 5
>>> print(a)
5
>>>
```

Note that using _print(a)_ has printed the value of 5 to us. So now if 
we wanted to add two numbers together, we can simply create a new 
variable _b_, give it a different value, and add them together using 
the + sign. See below:

```
Python 3.5.1 (v3.5.1:37a07cee5969, Dec  6 2015, 01:54:25) [MSC v.1900 64 bit (AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> a = 5
>>> print(a)
5
>>> b = 6
>>> print(a + b)
11
>>>
```
5+6 = 11, just as expected. 

We can also store the result of adding the numbers together in another 
variable _c_

```
Python 3.5.1 (v3.5.1:37a07cee5969, Dec  6 2015, 01:54:25) [MSC v.1900 64 bit (AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> a = 5
>>> print(a)
5
>>> b = 6
>>> print(a + b)
11
>>> c = a + b
>>> print(c)
11
```

We can see that _c_ now has the value 11 from the result of _a + b_

### Javascript Example
Navigate to jsfiddle.net

In the HTML pane to the top left, type the following code:
```
&lt;p id="output"&gt;&lt;/p&gt;
```

We'll use this for the rest of the examples as it provides a place for
us to see the output of the code that is written.

From now on, we'll be concentrating on the javascript pane to the bottom
left

Your browser should now look like the following:

![_config.yml]({{ site.baseurl }}/images/jsfiddle.png)

