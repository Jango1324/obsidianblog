---
title: October 29th Daily Recap
draft: false
tags:
  - school
  - physics
---
# Physics
So basically for torque, what it does is measuers the rotation of the stuff, the perpindicular has the most force while parallel has least

but remember there are angles and direction for force we just use sin as its vertical and stuff
for sign (+) or (-) it will be (-) for clockwise and (+) for anti clockwise, bascially thats it nothing crazy
also torque is 
TORQUE = LENGTH OF THE STUFF * FORCE



# Math
L'hopital's rule
bascially 
1) Put in the x = 0 ro infinity if you get (0/0 or infinity/infinity) then USE L'HOPITAL RULE
2) JUST TAKE DERIVATIVE OF THE TOP ONE AND DIVIDE BY DERIVATIVE OF THE BOTTOM ONE
   !!! DONT USE QUOTIENT RULE IN L'HOPITAL ITS IMPORTANT AF"
3) after you get the derivative plug in 0 or infinity and check again, if you still get (0/0) or (infinity/infinity) then keep going until x vanishes from denominator (bottom)

There are some sneaky shit in which you can use L'hopital for example you may re write this shit
ab = a/(b^-1) and then use l'hopital lol
why tf? cuz algebra makes it work because you keep change flip and you get ab
REMEMBER YOUR AIM IS TO GET 
									(∞/∞) OR (0/0)
REGARDLESS




# COMPUTER FLUENCY (JAVASCRIPT)
Basic javascript commands

## OUTPUT AND INTERACTION

|Command|Description|Example|
|---|---|---|
|`alert("message")`|Shows a popup alert box|`alert("Hello Zhangir!");`|
|`prompt("message")`|Shows a popup asking for user input|`let name = prompt("What's your name?");`|
|`confirm("message")`|Shows Yes/No dialog, returns `true` or `false`|`let proceed = confirm("Are you sure?");`|
|`console.log()`|Prints info to the browser console (used for debugging)|`console.log("Debug info");`|
|`document.write()`|Writes text directly to the web page (use only for testing)|`document.write("Welcome!");`|


## WORK WITH HTML AND JS

| Command                                    | Description                                        | Example                                                          |
| ------------------------------------------ | -------------------------------------------------- | ---------------------------------------------------------------- |
| `document.getElementById("id")`            | Selects an element by ID                           | `document.getElementById("title").innerText = "Hello";`          |
| `document.getElementsByClassName("class")` | Selects all elements with a class (returns a list) | `document.getElementsByClassName("box")[0].style.color = "red";` |
| `document.querySelector("selector")`       | Selects first element by CSS selector              | `document.querySelector(".menu").style.display = "none";`        |
| `document.querySelectorAll("selector")`    | Selects all elements matching a CSS selector       | `document.querySelectorAll("p")`                                 |
| `element.innerHTML`                        | Gets or sets inner HTML content                    | `document.getElementById("info").innerHTML = "<b>Welcome!</b>";` |
| `element.innerText`                        | Gets or sets plain text                            | `document.getElementById("info").innerText = "Welcome!";`        |
| `element.style.property`                   | Changes CSS directly                               | `document.getElementById("box").style.backgroundColor = "blue";` |


## DECLARING VRBLS

| Command | Description                                      | Example                 |
| ------- | ------------------------------------------------ | ----------------------- |
| `let`   | Creates a block-scoped variable                  | `let age = 18;`         |
| `const` | Creates a constant variable                      | `const PI = 3.14159;`   |
| `var`   | (Older way) Defines a variable (not recommended) | `var name = "Zhangir";` |


## MATH AND STRINGS
Bascially same as in JAVA

## WHEN USER CLICKS AND STUFF LIKE THAT
|Command|Description|Example|
|---|---|---|
|`element.onclick = function()`|Runs code when clicked|`btn.onclick = () => alert("Clicked!");`|
|`element.addEventListener("event", function)`|Attaches an event listener|`button.addEventListener("click", sayHi);`|
|`onmouseover`, `onmouseout`, `onchange`|Detect hover, leave, or change|`input.onchange = () => console.log("Changed!");`|

