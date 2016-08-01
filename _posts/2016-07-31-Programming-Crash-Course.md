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
These storage locations are called **variables**.
- They provide a way to encapsulate blocks of code into reusable pieces. 
The most primitive of these is normally in the form of a **function**.
- They provide a way to run a block of code N times. This functionality 
is provided either as a loop construct or a way for a function to call 
itself the requisite number of times (this is called recursion). We’ll 
cover **for and while loops**.

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

### Python Variables Example
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

### Javascript Variables Example
Navigate to jsfiddle.net

In the HTML pane to the top left, type the following code:
&lt;p id="output"&gt;&lt;/p&gt;

We'll use this for the rest of the examples as it provides a place for
us to see the output of the code that is written.

From now on, we'll be concentrating on the javascript pane to the bottom
left

Your browser should now look like the following:

![_config.yml]({{ site.baseurl }}/images/jsfiddle.png)

In the javascript pane, type the following code:

    function print(message) {
        var output = document.getElementById('output');
      output.innerHTML = output.innerHTML + "<br>" + message;
    }
    
    var a = 5;
    
    print(a);

Then press the run button at the top left, and you should see output 
like the image below:

![_config.yml]({{ site.baseurl }}/images/jsfiddle2.png)

Notice that the output pane on the bottom right now contains the value 
of the variable _a_ that we set.

```
var a = 5;
```

Tells javascript to assign the value of 5 to the variable named _a_. 
We can now use _a_ later on in the program whenever we need the value 
again. We can see this when we call _print(a)_ which is a simple 
function we have defined to display the value of a variable. Each time 
we use _print(a)_ or _print(something)_ a new line will be appended to
the right panel. We'll talk more about functions later. Just keep in 
mind for now that _print(something)_ is magic that makes a new line
of text appear in the righthand bottom pane.

Now if we wanted to add two numbers together, we can simply create a new
variable _b_, give it a different value, and add them together using
the + sign. See below:


    function print(message) {
	    var output = document.getElementById('output');
        output.innerHTML = output.innerHTML + "<br>" + message;
    }
    
    var a = 5;
    print(a);
    
    var b = 6;
    print(a + b);


Then press the run button at the top left, and you should see output 
like the image below:

![_config.yml]({{ site.baseurl }}/images/jsfiddle3.png)

Note that, in the output pane to the right, we see the initial value of 
_a_ as 5, and then right below it the value of _a + b_ printed. 

5 + 6 is 11, as expected.

We can also store the result of adding the numbers together in another
variable c. Type the following into jsfiddle:

    function print(message) {
	    var output = document.getElementById('output');
        output.innerHTML = output.innerHTML + "<br>" + message;
    }
    
    var a = 5;
    print(a);
    
    var b = 6;
    print(a + b);
    
    var c = a + b;
    print(c);

Then press the run button at the top left, and you should see output 
like the image below:

![_config.yml]({{ site.baseurl }}/images/jsfiddle4.png)

As you can see, the output on the right is now
    
    5
    11
    11

Demonstrating that _c_ holds the result of _a + b_

# Functions
Functions allow you to package up multiple lines of code that you may 
want to reuse more than once in a project. This allows us to write
utilities that can be used from anywhere in a program as well as 
avoiding copying and pasting code all over the place that will lead to 
bugs and having to fix the same problems in multiple places.

### Python function example
In python, we define a function with the **def** keyword. Each function 
has a name, and a set of **parameters** that can be sent to it each time 
we call it. You can think of a function as telling someone what to do, 
and then adding some more specific instructions. A request such as 
"I would like a grilled cheese with tomato" could be represented in 
Python as a function defined like so:

~~~ python
def make_grilled_cheese(include_tomato): #include_tomato is a parameter 
    if include_tomato:
        #do something special to include tomato
    else:
        #make the grilled cheese, but no tomato
~~~

We can call the make_grilled_cheese function in two different ways.
The first includes the tomato, and the second omits it:

~~~ python
make_grilled_cheese(False) #makes a grilled cheese without tomato
make_grilled_cheese(True) #makes a grilled cheese with tomato
~~~

When the make_grilled_cheese function is called as above, the value we
pass in sets the value of the _include_tomato_ parameter inside the
function, and we can then test if the caller would like tomato or not.

In our previous python examples, _print()_ was a function that we called
to see the values of our variables. This function is defined by the
python language, so we didn't actually have to **def** it.

~~~ python
a = 5
print(a)
~~~

In the code above, _a_ is the parameter passed to the print function.
print(X) takes whatever we pass in for X and prints it to the screen

Lets define our own function and call it. Open IDLE and fill out a 
function called double_a_number. It should look like the following:

    Python 2.7.10 (default, May 23 2015, 09:40:32) [MSC v.1500 32 bit (Intel)] on win32
    Type "copyright", "credits" or "license()" for more information.
    >>> def double_a_number(number):
        return number * 2
    
    >>> 

The function we have defined is called double_a_number, and it takes a
single number as a parameter. **return** sends a value back to the
caller, and in this case, the value it sends is whatever the caller
passed to the _number_ parameter multiplied by 2 as in the above 
_return number * 2_

Now that we have a function to call, lets call it and see if it does
what we expect

    Python 2.7.10 (default, May 23 2015, 09:40:32) [MSC v.1500 32 bit (Intel)] on win32
    Type "copyright", "credits" or "license()" for more information.
    >>> def double_a_number(number):
        return number * 2
    
    >>> a = 5
    >>> double_a_number(a)
    10
    >>> 

As in the previous example, we set the value of _a_ to 5 using _a = 5_
but now instead of just printing it out, we pass it to our 
double_a_number function. We then see that _double_a_number(a)_ returns
10 as expected, since we passed 5 in as the number parameter and it was
doubled.

We can also store the return value of a function for later use. Just 
like an assignment of _a = 5_, we do this like so:

    Python 2.7.10 (default, May 23 2015, 09:40:32) [MSC v.1500 32 bit (Intel)] on win32
    Type "copyright", "credits" or "license()" for more information.
    >>> def double_a_number(number):
        return number * 2
    
    >>> a = 5
    >>> double_a_number(a)
    10
    >>> b = 10
    >>> result = double_a_number(10)
    >>> print(result)
    20
    >>> 

Note that we're assigning the result of _double_a_number(10)_ to the
variable result by typing _result = double_a_number(10)_ 

After that we can print out the result of _double_a_number(10)_ by calling the 
print function on _result_ as shown above in _print(result)_

### Javascript function example
In javascript, we define a function with the **function** keyword. Each 
function has a name, and a set of **parameters** that can be sent to it 
each time we call it. You can think of a function as telling someone 
what to do, and then adding some more specific instructions. A request 
such as "I would like a grilled cheese with tomato" could be represented 
in Javascript as a function defined like so:

