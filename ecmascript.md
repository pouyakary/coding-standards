---
description: >-
  These standard is for JavaScript, TypeScript and JSX. While they are pretty
  much specific to the ECMAScript world; most of them can be used within other
  languages too.
---

# Writing JavaScript

### Don't use semicolons

Semicolons are good, but they are not needed in ECMAScript. You can read [this post on how to code without semicolons](https://mislav.net/2010/05/semicolons/). Truth is while semicolons are optional and good to be used because everyone is using them, they are really ugly and by omitting them your code looks just a lot better and therefore semicolons are ignored within this standard.

Also remember that because this standard is designed for semicolon-less codes, you don't have to think about the edge cases because this standard automatically protects you from those kinds of problems.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.57.38_am.png)

### Spaces

Use spaces in a good way. Use at least one space before and after each parenthesis, braces, curly braces. Have at least an space after comma in the array and object notations. And always have at least one space before and after each operator. Only in case of an object or array inside a parentheses don't use spaces in between and have them as: `({ })`

![](.gitbook/assets/screen_shot_1396-12-11_at_2.48.42_am.png)

### Functions

In functions have a space between the function name and it's parentheses. Also in the argument names and between the function's return type and braces. If your function got more than 80 character break it down to many lines like the Objective-C style and align the parameters under each other where : are all in one column. In this case remember to have a line between the function's declaration and start of your code.

![](.gitbook/assets/screen_shot_1396-12-11_at_2.57.43_am.png)

When writing arrow functions remember to always separate the body from the definition by breaking them to two separate lines and have the body indented by one level.

![Good](.gitbook/assets/screen_shot_1396-12-11_at_3.02.58_am.png)

![Bad](.gitbook/assets/screen_shot_1396-12-11_at_3.04.44_am.png)

![Bad](.gitbook/assets/screen_shot_1396-12-11_at_3.04.50_am.png)

If the arrow function has only one parameter, don't use parentheses. And in cases where the whole code is one line don't use braces.

### Variable & Constants

As a general rule try to define everything as constant, it's much more healthy code. Try to write the value of each variable / constant under them with a level of indentation. It makes your code much more organized and readable.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.11.12_am.png)

### Ternary Operator

When using ternary operator remember to always wrap the whole thing in a parentheses. Then write a first line with conditions and then after that write the ? : and \) like this example.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.10.37_am.png)

### JSX

JSX is a terrible element when it comes to readability and so you must be extra carful not to unleash the daemon underneath it. To write beautiful JSX use the Objective-C style of function parameters and align all the params with = under each other. Add extra spacing between names, = and the values and also keep the spacings within the the braces.

Remember that JSX is bad for readability so don't define anything within the braces. Use a string, number, variable or function call. But don't define a new function or calculate math and other stuff that can easily make your JSX a mess.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.21.11_am.png)

When returning a JSX don't use parentheses after the return statement. Use a tab character to move to the next column and then write your JSX with the tab's indentation. It's just way more beautiful and stylish:

The nice way to return a JSX with an extra tab after the return keyword and two tabs in the other lines to have the JSX formed beautifully.

![The nice way...](.gitbook/assets/screen_shot_1396-12-11_at_3.26.35_am.png)

![The ugly way of returning JSX](.gitbook/assets/screen_shot_1396-12-11_at_3.27.10_am.png)

### If

In if statements don't use braces if only one statement must happen. However use them if the condition is too big and the user might not be easily able to spot the statement. Remember that in case of long conditions break them to more than one line where the && or \|\| operators are at the end of the previous line and that both statements start at one character column \(notice the this.lastStates\)

![](.gitbook/assets/screen_shot_1396-12-11_at_3.31.10_am.png)

### Switch

In writing switches only notice to have the cases be indented by one level in the main switch body.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.35.14_am.png)

### Objects

If you're cloning an object with spread operator use the spread operator ofter the beginning of the object within the first line. Then remember to use enough tabs ofter the object keys that their values be aligned under a new column.

![](.gitbook/assets/screen_shot_1396-12-11_at_3.39.49_am.png)

When you have nested objects within the object you're defining make an empty line and then define the nested object. And have all the single value objects on the top of the object declaration

![](.gitbook/assets/screen_shot_1396-12-11_at_3.43.11_am.png)

### Kary Comments

Kary Comments are a core building block of this coding style. When we write notes or documents, etc. we use horizontal dividers to separate parts of our document. That must happen within our codes too.

Kary Comments are simply horizontal dividers with a little bit of style. You don't have to write them with hands. There are many tools available already. Check out:

Kary Comments

![](.gitbook/assets/screen_shot_1396-12-11_at_12.38.00_pm.png)

