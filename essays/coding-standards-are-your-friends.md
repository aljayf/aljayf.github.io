---
layout: essay
type: essay
title: Coding Standards are Your Friends
# All dates must be YYYY-MM-DD format!
date: 2018-09-20
labels:
  - Learning

---
<img class="ui medium right floated rounded image" src="../images/ESLint.png">
<h2>A Little Boost</h2>
If you are coding, it is to your best interest to implement coding standards. Following coding standards allows code to maintain uniformity. In result, your code becomes more readable as it presents a common look and feel thus allowing it to scale beyond one person. One may think of coding standards as a trivia way to know how many spaces to indent or to place a close-curly-brace on a new line by itself, but I believe coding standards can improve quality and can actually help you learn a programming language. In the process of learning a new programming language, you make mistakes. Without coding standards and the tools to enforce them, you may not be aware of these mistakes. What could be a little mistake could also be a big problem in programming. However, coding standards may point out these mistakes as soon as you make them.

<h2>First Impressions</h2>
In my first week of using ESLint with IntelliJ, I thought that it was neat and helpful. As I wrote code, I would get error messages on my coding style. At first, I did not agree with them since that was how I always written my code. However, when I followed the suggestions to fix the error, I had to admit that the code was more readable. Using ESLint with IntelliJ did more than recommend me to add a space. It also, recommended me to use a different type of assignment statement. 
```
let a = 1;
let b = 2;
a = a + b;
```
This code is works fine, but ESLint with IntelliJ forced me to write the assignment statement as follows:
```
let a = 1;
let b = 2;
a += b;
```
I was quite impressed that it told me I could do the same thing, but in a better way. 

<h2>Green Check</h2>
Throughout my first week of using ESLint, I thought that getting the green checkmark was both painful and useful. The first time I tried to get the green checkmark was a pain. I had to rearrange my code and change a few assignment statements, but this was useful. It allowed me to become a better programmer as I got a better understanding of writing cleaner code.
