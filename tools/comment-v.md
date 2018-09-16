---
description: Comment V is a Kary Comments Generator for Visual Studio Code.
---

# Comment V for Visual Studio Code

{% hint style="danger" %}
You are reading a draft edition of this document. If you found any errors, please report them to [kary@gnu.org](mailto:kary@gnu.org)
{% endhint %}

Comment V is the most user-friendly implementation of Kary Comment Generators \(KCGs\). Unlike the previous versions \(III, IV\); Comment V is an editor extension and as a result it knows the environment of the code, it know the language, indentation settings, et cetera and therefore with push of a button it is able to write the desirable comment for you.

![A demo of Comment V in KaryScript](../.gitbook/assets/28877787-ace1415e-77b2-11e7-81fa-e4d3d7af50ec.gif)

## How It Works?

1• Start a new empty line and write a title for your comment there

![](../.gitbook/assets/screen-shot-1397-06-25-at-12.12.18-am.png)

2 • Push `y` while holding `alt` and you see the line becoming a section comment:

![](../.gitbook/assets/screen-shot-1397-06-25-at-12.14.06-am.png)

3 • Notice the extra lines and the indentation. Comment V creates enough space for you to reach where you should write your code. So; write your code.

![](../.gitbook/assets/screen-shot-1397-06-25-at-12.15.48-am.png)

## Available Commands

| Comments | Keybindings | Additional Information |
| :--- | :--- | :--- |
| Flag | `alt` + `shift`+ `y` | You'll have to also give it the index number |
| Section Header | `alt` + `y` | Section Comment for Indentation less than 2 and InSection comment for the rest |
| Reverse Section Start | `alt` + `m` | _same as section comment_ |
| Section End | `alt` + `l` | Line Comment for Indentation less than 2 and Separator comment for the rest |

## Supported Comments

```text
──
── ─── INDENTATION LEVEL 1 ────────────────────────────────────────────────────────
──

──
── ─────────────────────────────────────────────────── REVERSE SECTION HEADER ─────
──

        ──
        ── ─── INDENTATION LEVEL 2 ─────────────────────────────────────────
        ──

        ──
        ── ──────────────────────────────────── REVERSE LEVEL 2 HEADER ─────
        ──

                ──
                ── INDENTATION LEVEL 3
                ──

                ── • • • • •

        ── ─────────────────────────────────────────────────────────────────

── ────────────────────────────────────────────────────────────────────────────────
```



