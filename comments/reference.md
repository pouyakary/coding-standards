---
description: This page explains all the comments and their usage
---

# Comments Reference

## Section and Line Comments

The **Section** and **Line** comments are a pair comment to be used as a group. The line comment is designed to draw a line between parts of the code so that you can read the code with ease. Then section comment combines the line comment with a _one line comment_ — like `// something` — to title the sections. Take this code as an example:

```javascript
// Loading the File 
function LoadFile ( ) {
   ...
}

// Storing the File
function StoreFile ( ) {
   ...
}
```

You can comment this code like this:

```javascript
//
// ─── FILE LOADER ──────────────────────────────────────────────────────
//

    function LoadFile ( ) {
        ...
    } 

//
// ─── FILE STORER ──────────────────────────────────────────────────────
//

    function StoreFile ( ) {
        ...
    }

// ──────────────────────────────────────────────────────────────────────
```

{% hint style="success" %}
Notice the empty lines above and under the function comment as well as the 1 level indentation of the codes inside the sections
{% endhint %}

## Level 2 Sections

Level 2 Sections are Section Comments of size **60** chars \(the section comment is **80** chars\). A level 2 Section Comment is used to divide a Section into smaller parts. For examples. Many times; A Class is itself a section in a much bigger code. In cases such as this we use Sub Sections to divide the class.

```javascript

//
// ─── MY CLASS ───────────────────────────────────────────────────────────────────
//

    class Something extends SomethingElse {
    
        //
        // ─── CONSTRUCTOR ────────────────────────────────────────────
        //
    
            constructor ( ...arguments ) {
                super( ...arguments )
            }
            
        //
        // ─── HELLO ──────────────────────────────────────────────────
        //
        
            hello ( ) {
                console.log( "Hello, World" )
            }
    
        // ────────────────────────────────────────────────────────────
        
    }

// ────────────────────────────────────────────────────────────────────────────────

```

{% hint style="success" %}
In order to generate this comment in Comment V \(or any other KCG in editors\) you have to use the standard section command and the generator automatically sets the kind SubSection based on indentation
{% endhint %}



In order to generate this comment in Comment V \(or any other KCG in editors\) you have to use the standard section command and the generator automatically sets the kind InSection based on indentation

## InSection Comments

InSection Comments are used when you reach the sectioning limit \(Sections &gt; 2\). In these cases you can go on dividing by the InSection comments.

```javascript
                    //
                    // SOME KIND OF A TASK
                    //
```

{% hint style="success" %}
In order to generate this comment in Comment V \(or any other KCG in editors\) you have to use the standard section command and the generator automatically sets the kind InSection based on indentation
{% endhint %}

{% hint style="danger" %}
Reaching this comment is a sign of bad code. Try to divide your code to simpler and smaller units.
{% endhint %}

## Flag Comments

A **flag comment** is used to point the major divisions within your code. For example say you have a GUI app on just one file. Then your MVC model will be divided to:

```javascript
//
// ────────────────────────────────────────────────── I ──────────
//  :::::: M O D E L : :  :   :    :     :        :          :
// ────────────────────────────────────────────────────────────
//

//
// ─── MODEL FUNC 1 ─────────────────────────────────────────────────────
//

   function ModelFunc1 ( ) { 
      ...
   }

//
// ─── MODEL FUNC 2 ─────────────────────────────────────────────────────
//

   function ModelFunc2 ( ) { 
      ...
   }

// ──────────────────────────────────────────────────────────────────────





//
// ──────────────────────────────────────────────── II ──────────
//  :::::: V I E W : :  :   :    :     :        :          :
// ──────────────────────────────────────────────────────────
//

//
// ─── VIEW FUNC 1 ──────────────────────────────────────────────────────
//

   function ViewFunc1 ( ) { 
      ...
   }

//
// ─── VIEW FUNC 2 ──────────────────────────────────────────────────────
//

   function ViewFunc2 ( ) { 
      ...
   }

// ──────────────────────────────────────────────────────────────────────





//
// ──────────────────────────────────────────────────────────── III ──────────
//  :::::: C O N T R O L L E R : :  :   :    :     :        :          :
// ──────────────────────────────────────────────────────────────────────
//

//
// ─── CONTROLLER FUNC 1 ────────────────────────────────────────────────
//

   function ControllerFunc1 ( ) { 
      ...
   }

//
// ─── CONTROLLER FUNC 2 ────────────────────────────────────────────────
//

   function ControllerFunc2 ( ) { 
      ...
   }

// ──────────────────────────────────────────────────────────────────────
```

{% hint style="success" %}
A good thing about flags is that they are immensely big and therefore easy to spot in the mini maps.
{% endhint %}

{% hint style="danger" %}
Flags are are not first-class fundamentals because they are designed for very big files \(say more than 750~1000 lines of code\) and Kary Coding Standards does not encourage the use of big files. It is rather recommended to use many files and keep them small so that the organization of your codes remain well.
{% endhint %}

## Deprecated Comments

Before reaching to a stable version of the standards; there used to be many other comments. Namely:

* Class Comments
* Legacy SubSection Comments
* Legacy SubLine Comments

While they are still included in older versions of comment \(III/IV\), they are deprecated in this standards. You can use them for fun but they are not encouraged by this standards.

