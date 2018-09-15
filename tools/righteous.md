---
description: An experimental CSS formatter that implements the Kary Coding Standard
---

# Righteous — CSS Formatter

![Your humble witch](../.gitbook/assets/framed-head.png)

Righteous is a formatter for CSS that implements Kary Coding Standards. It is written as a reconstructing formatter; It means righteous parses the code into an AST \(abstract syntax tree\) and then rewrites that tree to CSS. This technique ensures everything is based on the standard.

### Righteous for Visual Studio Code

Currently—and till reaching a stable release—Righteous is only available as a preview Visual Studio Code. Righteous is being used in some production projects to be tested and when ensured, it'll be released for other editors too.

[**Install Righteous for Visual Studio Code**](https://marketplace.visualstudio.com/items?itemName=karyfoundation.righteous)\*\*\*\*

![Righteous overrides the default formatter and silently beautifies your code for you](../.gitbook/assets/righteous-demo.gif)

### Righteous Core for Developers

In case you want to have Righteous working in other tools and editors, You can easily do so by getting the npm package `righteous-core`

```javascript

//
// ─── IMPORTS ────────────────────────────────────────────────────────────────────
//

    const righteous = require('righteous-core')

//
// ─── BODY ───────────────────────────────────────────────────────────────────────
//

    const code = "h1 { color: red }"

    try {
        // Righteous is a simple function, you feed
        // it source code and it returns the formated 
        // one
        const formattedCode = righteous( code )
        
    } catch ( e ) {
        // also keep in mind that on parse failiure
        // or unsupported tokens, it'll throw you errors
        // so always have the try/catch
        throw e
    }
    
// ────────────────────────────────────────────────────────────────────────────────

```

