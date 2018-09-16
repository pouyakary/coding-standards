---
description: >-
  Languages that have specification in this standard; already have sound detail
  on how to use the Kary Comments. What this documents tries to do, is how to
  use the tools in any language.
---

# Sectioning Code

{% hint style="danger" %}
You are reading a draft edition of this document. Please if you found any errors, report them to [kary@gnu.org](mailto:kary@gnu.org)
{% endhint %}

## What a Section Comment is?

A section comment is a Kary Comment that names the section. See in this example how section comments have separated the parts. 

![](../.gitbook/assets/screen-shot-1397-06-25-at-2.38.02-am.png)

When dealing with a very long section; A "Reverse Section Comment" can be utilized to indicate the ending of that section

![](../.gitbook/assets/screen-shot-1397-06-25-at-2.43.25-am.png)

At the end of a series of sections, A line comment is used to decorate

![](../.gitbook/assets/screen-shot-1397-06-25-at-2.45.37-am.png)

## Indentation of Sections

In indentation sensitive language such as Python and Haskell, a compact version of Kary Comments is used. You can see that in space sensitive languages section comments are one line and in the insensitive they are 3 lines:

```text

//
// ─── TITLE ──────────────────────────────────────────────────────────────────────
//

# ─── TITLE ──────────────────────────────────────────────────────────────────────

```

But also in case insensitive languages, there is a level of indentation introduced after using the section comment as this:

![](../.gitbook/assets/screen-shot-1397-06-25-at-2.37.07-am.png)

{% hint style="warning" %}
Kary Coding Standard is based on the idea of 4 space tabs. It is also important to write codes with spaces to keep the layout the same everywhere.
{% endhint %}





