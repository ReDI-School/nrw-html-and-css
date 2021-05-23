---
title: Lesson 17 - CSS Overflow and Text Effects
nav_order: 17
---

# CSS Overflow and Text Effects

## Class Agenda

1. CSS Overflow
2. CSS Text Effects

# 1. Overflow

There are many scenarios in which the content of an html tag is simply bigger than the size of the html tag container itself. This makes the content overflow.

Students would learn about the default `overflow` behaviour and the principle which CSS applies to ["avoid data loss"](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Overflowing_content#css_tries_to_avoid_data_loss).

Apart from that, the section covers the CSS `overflow` rule. Students would learn about the different values possible to be added to overflow:

- `visible`
- `hidden`
- `clip`
- `scroll`
- `auto`

Furthermore, this section covers the different directions an overflow can happen. These are `overflow-x` and `overflow-y`. Additionally, the students would learn the requirements for the `overflow` property to work properly. All of this would be taught with practical examples.

ETA: 40 min

# 2. Text Effects

What should we do when we have long words? Should we use scrolling with `overflow-x` ? In this section students would learn alternative and perhaps better approaches to deal with the former problem. This includes covering the [CSS Text Effects](https://www.w3schools.com/css/css3_text_effects.asp) and the respective CSS rules associated with them. These are:

- `text-overflow`
- `overflow-wrap` (`word-wrap`)
- `word-break`
- `line-break`
- `writing-mode`

Some of these rules are very similar but yet distinct enough. The lecture would cover in details the differences between:

- `word-break: break-all` versus `overflow-wrap: break-word` in CSS
- `word-wrap` and `overflow-wrap`
- `line-break` and `word-break`

ETA: 40min

# Glossary & Terminology

# Homework

1. The usage of overflow and text effects is more situational. Please practice using these rules on your website but do not necessarily include these rules in your websites. That is why we also do not have a fixed checkpoint.

2. Read the following [article](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Sizing_items_in_CSS) which is a recap of different ways to size items in CSS

Make sure to ask questions!

# Resources

- [How to deal with long words?](https://justmarkup.com/articles/2015-07-31-dealing-with-long-words-in-css/)
- [MDN CSS Overflowing Content Tutorial](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Overflowing_content)
- [MDN CSS Overflow rule](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow)
