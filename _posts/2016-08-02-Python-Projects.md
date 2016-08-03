---
layout: post
title: Python Projects
---

Dinner and Code currently offers two programming paths: Python and web development. On this page are the Python projects.

Python is a modern, interactive, object oriented programming language. Its clear 
syntax and extensive libraries make it a great choice for beginners that 
want to learn to write code without having to write absolutely everything 
on their own.

# Project Listing
Project 1: Dice Rolling Game

Project 2: Mad Libs Generator

Project 3: Hangman


# Project 1: Dice Rolling Program
Difficulty Level: Beginner

Language: Python

## Concepts Learned:
<ul>
<li>Using a text editor and console</li>
<li>Importing a module</li>
<li>Creating a WHILE loop</li>
<li>Working with Integers</li>
<li>Print</li>
</ul>

## Description:
This basic dice rolling program will let you get comfortable with coding in Python. The
program will randomly select a number (based on the number of “sides” your die
has) and print it out on the screen. 

## What you’ll need:

### Text editor such as:

1. NotePad++ ([https://notepad-plus-plus.org](https://notepad-plus-plus.org/))

2. Brackets ([http://brackets.io/](http://brackets.io/)) 

3. TextWrangler ([http://www.barebones.com/products/textwrangler/](http://www.barebones.com/products/textwrangler/)) 

### Python Download:
[Python Download Page](http://python.org/download)

### Learning Resources for this Lesson:
<ul>
<li>How to Use the Random Module in
Python[http://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python](http://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)</li>
<li>Choose Your on PyVenture: The Random
Module [https://en.wikibooks.org/wiki/Choose_Your_Own_Pyventure/Random_and_PRNGs](https://en.wikibooks.org/wiki/Choose_Your_Own_Pyventure/Random_and_PRNGs)</li>
<li>Learn Python the Hard Way (Python
2.7) [http://learnpythonthehardway.org/](http://learnpythonthehardway.org/)</li>
<li>Zed Shaw’s Command Line Crash Course [http://learnpythonthehardway.org/book/appendixa.html](http://learnpythonthehardway.org/book/appendixa.html)</li>
<li>Python 2.7 Docs [https://docs.python.org/2.7/](https://docs.python.org/2.7/)</li>
</ul>

### The How-To Video for this Project
[YouTube](https://youtu.be/48n9NnK4k-M)


## The Steps
### Step 1: Get Set Up
You’ll need to install a text editor and configure it for your particular machine. Since
the steps vary, it’s best to do some Google Fu as it relates to your particular
text editor + OS combination. 

See: [http://learnpythonthehardway.org/book/ex0.html](http://learnpythonthehardway.org/book/ex0.html)

You’ll then need to install Python 2.7:

[http://python.org/download](http://python.org/download)


### Step 2: Create a file in your Text editor

Go ahead and create a .py file in your editor. This file is what you’ll call in your command
line. Make sure you save it in the right place so Python can call it up.

### Step 3: Start writing some code

This program has several components:

1.    Call the Random Module

2.    Define a function to Roll the dice

3.    Define a main() function of the
program

4.    Print the results


Code
Example:

import
random

 

def
roll(sides=6): 

    num_rolled = random.randint(1,sides)

    return num_rolled

 

def main():

    sides = 6

    rolling = True

    while rolling:

        roll_again = input("Ready to roll?
ENTER=Roll. Q=Quit. ")

        if roll_again.lower() != "q":

        num_rolled = roll(sides)

        print("You rolled a",
num_rolled)

    else:

        rolled = False

        

    print("Thanks for playing.")

    

    main()

 

**

### Step 4: Run the program

In your command line, go ahead and run the program. If you need help, see: [http://learnpythonthehardway.org/book/ex1.html](http://learnpythonthehardway.org/book/ex1.html)

