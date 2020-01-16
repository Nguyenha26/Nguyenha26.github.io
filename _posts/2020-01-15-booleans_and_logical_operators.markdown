---
layout: post
title:      "Booleans and Logical operators"
date:       2020-01-15 12:38:34 -0500
permalink:  booleans_and_logical_operators
---


Boolean expressions allow programmers to write programs that help decide whether some code will be executed or not. The decisions will change the flow of the program based on whether the expressions are true or false. Before diving into a lab that involves booleans, a great question to ask is: What is a Boolean? 

A boolean is a “value used in a logical statement to say if something is considered true or false. In order to return true or false values, booleans use two types of operators: Rational and Logical. Rational operators compares two arithmetic expressions and uses boolean help determine the results. Here are six frequently used rational operators:


* (equal to) == 
* (not equal to) !=
* (less than) < 
* (less than or equal to) <=
* (greater than) >
* (greater than or equal to) >=

Logical operators combine boolean values and evaluate to a boolean result. Here are the 3 main logical operators: 

* ! (“Single-bang”) which represents “NOT”
* && (“double-ampersand”) which represents “AND”
* | | (“double-pipe”) represents “OR” 

In this lab, we will be using logic operators and conditional statements (if, elsif, else) to solve it. 

**LAB ACTIVITY**

Write a speak_to_grandma method.

Whatever you say to grandma, she should respond with
HUH?! SPEAK UP, SONNY!
unless you shout it (type in all capitals).

If you shout, she can hear you (or at least she thinks so) 
and yells back:NO, NOT SINCE 1938!

However if you say 'I LOVE YOU GRANDMA!', she should respond with
I LOVE YOU TOO PUMPKIN!'




*First create a method (def, end) using a method signature of “speaktograndma. Right after the method signature, we will list an argument “(what is in between the parenthesis) at the end.*

**def speak_to_grandma (phrase)**
 
*There are 3 parts to grandma’s response, and based on whether she hears, may have heard, or doesn’t it will return the following phrases:

If grandma does hear you she would say: “I LOVE YOU TOO PUMPKIN”
If grandma doesn’t hear you, she would respond: “HUH?! SPEAK UP, SONNY!”
If grandma thought she heard what you said, she would respond: “NO, NOT SINCE 1938!”

Now we are going to construct the conditional statements (if, elsif, else). 

If grandma heard “I LOVE YOU GRANDMA!” we are going to build the “if” statement like this: (the “.upcase” is used to capitalize the string). The “puts” is going to be grandma’s response “I LOVE YOU TOO PUMPKIN!”*

**if speak_to_grandma == "I love you grandma!".upcase
 		puts "I love you too pumpkin!".upcase**

*Over the years, grandma’s hearing level has decreased. If she didn’t hear what you said, her response would be “HUH?! SPEAK UP, SONNY!” Because it wasn’t clear, we would build the “elsif” statement to represent that she didn’t hear our response.*

**elsif speak_to_grandma == "You're awesome grandma.".upcase
  		puts "Huh?! Speak up, sonny!".upcase**

*However, let’s say if grandma hear us and THOUGHT it was a different response than ‘I LOVE YOU GRANDMA” than we would create the “else” statement. *

**else 
  		puts "No, not since 1938!".upcase
end
**


(https://www.rubyguides.com/2019/02/ruby-booleans/)
(https://www.cs.cmu.edu/~mrmiller/15-110/Handouts/boolean.pdf)

