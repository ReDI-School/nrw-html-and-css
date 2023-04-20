---
title: Lesson 10 - CSS Flexbox
nav_order: 10
---

# CSS Flexbox

## Class Agenda

1. Introduction to Flexbox
1. The Flex model

## 1. Introduction to Flexbox

Flexbox is a comparatively newer way to layout elements on the page without the limits and frustration of Floats like:

- You have to clear Floats (when the containing element collapses).
- Sometimes have to change the order of your HTML to achieve a Floats design.

Flexbox layout makes it easier to design flexible responsive layout structure (hint: Flexbox = flexible boxes).

With flexbox, you can align elements horizontally and vertically. Unlike floats, you can re-order flex items without needing to change the HTML.

## 2. The Flex Model

- `flex` is the value for the display property that activates the Flexbox layout on an element.
- What is a flex container?
- What are flex items?
- What are the most common properties that can be used on a flex container?
  - `flex-direction` (default `row`)
  - `flex-wrap` (default `nowrap`)
  - `justify-content` (default: `flex-start`)
  - `align-items` (default: `stretch`)
  - `align-content` (default: `stretch`)
  - `flex-flow`
- What are the most common properties that can be used on a flex item?
  - `align-self` is similar to `align-items` on the container, but applies to a single flex item.
  - `flex`: shorthand property for the `flex-grow`, `flex-shrink`, and `flex-basis`
  - `flex-grow`: specifies how an item grows when it is allowed to take extra space available in the container (default: 0)
  - `flex-shrink` specifies how an item shrinks when there is not enough space available in the container (default: 1)
  - flex-basis
  - order

## [Example](https://codepen.io/redi-school/pen/eYPJzRY)

## Exercises

1. Practice using Flexbox with this [codepen](https://codepen.io/redi-school/pen/jOeWrvj)
2. [Flexbox Froggy](https://flexboxfroggy.com/)

## [Quiz](https://create.kahoot.it/creator/aee4f0bd-34b4-451d-ae52-c6f7d1563dd8)

## Homework

Finish the above exercises, otherwise try and implement Flexbox into your project websites.

# Glossary

- Flexbox - Flexible box

# Resources

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
