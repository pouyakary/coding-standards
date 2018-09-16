---
description: >-
  These specifications are for JavaScript, TypeScript and JSX. While they are
  pretty much specific to the ECMAScript world; most of them can be used within
  other languages too.
---

# JavaScript Family

{% hint style="info" %}
You are reading a draft edition of this document. Please if you found any errors, report them to [kary@gnu.org](mailto:kary@gnu.org)
{% endhint %}

## Don't use Semicolons

Semicolons are good, but they are not needed in ECMAScript. You can read [this post on how to code without semicolons](https://mislav.net/2010/05/semicolons/). Truth is while semicolons are optional and good to be used—since everyone is using them—they are really ugly. By omitting them your code looks just a lot better and thus semicolons are ignored within this standard.

{% hint style="success" %}
Because this standard is designed for semicolon-less codes, you don't have to think about the edge cases since this standard automatically protects you from those kinds of problems.
{% endhint %}

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.57.38_am.png)

## Spaces

Use spaces in a good way. Use at least one space before and after each parenthesis, braces, and curly braces. Have at least an space after comma in the array and object notations. And always have at least one space before and after each operator.

Only in case of an object or array inside a parentheses don't use spaces in between and have them as: `({ })`

![](../.gitbook/assets/screen_shot_1396-12-11_at_2.48.42_am.png)

{% hint style="warning" %}
In Kary Coding Standards the standard size for a tab is 4 spaces and they must be written by spaces to keep the look of the code
{% endhint %}

{% hint style="warning" %}
You don't have to use space before the `(`of a function call. So `foo( )` not `foo ( )`
{% endhint %}

## Functions

In functions have a space between the function name and it's parentheses. Also in the argument names and between the function's return type and braces.

If your function has more than 80 character break it down to many lines like the Objective-C style and align the parameters under each other where `:` are all in one column. In this case remember to have a line between the function's declaration and start of your code.

![](../.gitbook/assets/screen_shot_1396-12-11_at_2.57.43_am.png)

When writing arrow functions remember to always separate the body from the definition by breaking them into two separate lines and have the body indented by one level

![Good](../.gitbook/assets/screen_shot_1396-12-11_at_3.02.58_am.png)

![Bad](../.gitbook/assets/screen_shot_1396-12-11_at_3.04.44_am.png)

![Bad](../.gitbook/assets/screen_shot_1396-12-11_at_3.04.50_am.png)

If the arrow function has only one parameter, don't use parentheses. And in cases where the whole code is one line don't use braces.

## Variable & Constants

As a general rule, try to define everything as constant. it's much more healthy code. Try to write the value of each variable / constant under them with a level of indentation. It makes your code much more organized and readable.

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.11.12_am.png)

## Ternary Operator

When using ternary operators, remember to always wrap the whole thing in parentheses. Then write a first line with conditions and then after that write the `?` `:` and `)` like this example.

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.10.37_am.png)

## JSX

JSX is a terrible element when it comes to readability and so you must be extra carful not to unleash the daemon underneath it. To write beautiful JSX use the Objective-C style of function parameters and align all the params with `=` under each other. Add extra spacing between names, `=` , and the values and also keep the spacings within the the braces.

Remember that JSX is bad for readability so don't define anything within the braces. Use a string, number, variable or function call. But don't define a new function or calculate math and other stuff that can easily make your JSX a mess.

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.21.11_am.png)

When returning a JSX, don't use parentheses after the return statement. Use a tab character to move to the next column and then write your JSX with the tab's indentation. It's just way more beautiful and stylish:

The nice way to return a JSX with an extra tab after the return keyword and two tabs in the other lines to have the JSX formed beautifully.

![The nice way of returning JSX](../.gitbook/assets/screen_shot_1396-12-11_at_3.26.35_am.png)

![The ugly way of returning JSX](../.gitbook/assets/screen_shot_1396-12-11_at_3.27.10_am.png)

## Control Structures

In these control structures don't use braces if only one statement must happen. However, use them if the predicate is too big and the user might not be easily able to spot the statement. Remember that in the case of long conditions break them to more than one line where the `&&` , `||` , and `;`  operators are at the end of the previous line and that both statements start at one character column \(notice the `this.lastState`s\)

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.31.10_am.png)

### Switch

In writing switches, only notice to have the cases be indented by one level in the main switch body.

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.35.14_am.png)

## Objects

If you're cloning an object with spread operator, use the spread operator ofter the beginning of the object within the first line. Then remember to use enough tabs ofter the object keys that their values be aligned under a new column.

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.39.49_am.png)

When dealing with nested objects within the object you're defining, make an empty line and then define the nested object. Make sure to have all the single value objects on the top of the object declaration

![](../.gitbook/assets/screen_shot_1396-12-11_at_3.43.11_am.png)

## Kary Comments

Kary Comments are a core building block of this coding standard. When one writes notes or documents, etc. it uses horizontal dividers to separate parts of its document. That must happen within codes too.

Kary Comments are simply horizontal dividers with a little bit of style. You don't have to write them with hands. There are many tools available already. Check out:

{% page-ref page="../comments/introduction.md" %}

{% page-ref page="../comments/sectioning.md" %}

![](../.gitbook/assets/screen_shot_1396-12-11_at_12.38.00_pm.png)

## Array

To define arrays use the very standard way of defining them. Don't break lines in the definition.

![](../.gitbook/assets/screenshot1397-02-29at11.52.33am.png)

## Types

JavaScript does not provide any static typing facilities but thanks to TypeScript and Flow, it is now possible to have these functionalities in one's codes. This document assumes you're using TypeScript but Flow is almost the same, so all the concepts are easy to apply there too.

### **Naming Types**

![](../.gitbook/assets/screen-shot-1397-06-24-at-6.03.18-pm.png)

### **Interfaces**

In interfaces, like objects, use the column style and keep keys and values in separate columns. Also remember not to use any semicolon in interfaces

![](../.gitbook/assets/screenshot1397-02-29at12.04.06pm.png)

### **Declaring Types**

When declaring types don't use too much comments. Also, using column-style is very much rewarded because these types are usually very compressed and it's always great to make them more readable.

![](../.gitbook/assets/screenshot1397-02-29at12.08.21pm.png)

### **Type Annotations**

When defining types remember to have no spaces before `:` and at least one space after it.

![](../.gitbook/assets/screenshot1397-02-29at12.11.34pm.png)

## Class

The only tricky part of a class is the use of Kary Comments inside of it. Comments inside of a class must be of length 60. If you're using a comment generator inside of your editors, they will automatically set the length.

![](../.gitbook/assets/screenshot1397-02-29at1.42.12pm.png)

## Documentation Comments

Documentation comments can easily live alongside Kary Comments but the idea is to not use them alone.

![](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3e77bac6-5e20-4bb2-9be2-6badefad45ce/ScreenShot1397-02-29at1.48.30PM.png?AWSAccessKeyId=AKIAJLJXUMP5IHUZAPFQ&Expires=1537105102&Signature=ZVqfBjohjYA%2BD7iEXAAFtEVpabI%3D)

## Imports

When it comes to writing writing ES6 module loaders, try to keep the column-based approach if possible.

![](../.gitbook/assets/screenshot1397-02-29at1.51.42pm%20%283%29.png)

When using the deconstructing assignment remember to keep one space around braces

![](../.gitbook/assets/screenshot1397-02-29at1.54.21pm.png)

## Namespaces

TypeScript provides a great namespace feature that when combined with AMD/system bundlers makes TypeScript an amazing choice. To use namespaces you have to use the namespace system and the reference paths. Here we discuss the styling for this system.

![](../.gitbook/assets/screenshot1397-02-29at12.25.38pm.png)

Namespace must be defined on the root of the code and then you have to give it one level of indentation for Kary Section Comment and then one more level of indentation for the comments.

Keep reference paths one/two lines above the namespace and below your code comments to give them their true import statement look.

