---
title: Lesson 14 - CSS Layout 2 - Flexbox
nav_order: 14
---

## Class Agenda

1. Introduction to Flexbox
1. The Flex model

## 1. Introduction to Flexbox

Flexbox is a comparatively newer way to layout elements on the page without the limits and frustration of Floats like:
  - You have to clear Floats (when the containing element collapses).
  - Sometimes have to change the order of your HTML to achieve a Floats design

Flexbox layout makes it easier to design flexible responsive layout structure (hint: Flexbox = flexible boxes).

With flexbox, you can align elements horizontally and vertically. Unlike floats, you can re-order flex items without needing to change the HTML

## 2. The Flex Model

- `flex` is the value for the display property that activates the Flexbox layout on an element.
- What is a flex container?
- What are flex items?
- Explain some properties that can be used on a flex container
  - `flex-direction` (default `row`)
  - `flex-wrap` (default `nowrap`)
  - `justify-content` (default: `flex-start`)
  - `align-items` (default: `stretch`)
  - `align-content` (default: `stretch`)
  - `flex-flow`
- Explain some properties that can be used on a flex item
  - `align-self`, similar to `align-items` on the container, but applies to a single flex item.
  - `flex`: shorthand property for the `flex-grow`, `flex-shrink`, and `flex-basis`
  - `flex-grow`: specifies how an item grows when they're allowed to take extra space available in the container (default: 0)
  - `flex-shrink` specifies how an item shrinks when there is not enough space available in the container (default: 1)
  - flex-basis
  - order


# Exercise Description
1. Layout the navigation bar on the portfolio with Flexbox
2. Style the Flexible single line form in the HTML provided
3. Style the Flexbox Pricing Grid in the HTML provided

# Homework

- Checkpoint 14

# Resources

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
