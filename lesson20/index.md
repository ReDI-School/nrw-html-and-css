---
title: Lesson 20 - CSS Selectors II
nav_order: 18
---

# CSS Selectors II

This lesson teaches various CSS Selectors which are not so often used but still important. The theory would be accompanied with practical examples for each selector case.

## Class Agenda

1. Recap of the CSS Selectors I
2. CSS Combinator Selectors
3. CSS Pseudo Classes
4. CSS Pseudo Elements
5. CSS Attribute Selectors

# 1. Recap of the CSS Selectors I

We have written a decent amount of CSS rules for our website so far. While the amount of CSS rules is high, we have not used too many different CSS Selectors for our rules. We have mainly used the Simple CSS Selectors such as

- the CSS element Selector
- the CSS id Selector
- the CSS class Selector
- the CSS universal Selector
- and others

We have covered those selectors during our [introduction CSS lecture](https://redi-school.github.io/nrw-html-and-css-2021-spring/lesson8/#3-css-selectors-i). Apart from that, we have also covered the CSS Descendant Selector which belongs to the group of Combinator Selector during another one of our [CSS lectures](https://redi-school.github.io/nrw-html-and-css-2021-spring/lesson9/#1-css-descendant-selector). The main goal of lesson 20 is to cover the rest of the CSS Selectors, so that the we learn more possibilities to style our websites.

2. CSS Combinator Selectors
3. CSS Pseudo Classes
4. CSS Pseudo Elements
5. CSS Attribute Selectors

# 2. CSS Combinator Selectors

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

- descendant selector (space)
- child selector (>)
- adjacent sibling selector (+)
- general sibling selector (~)

# 3. CSS Pseudo Classes

A pseudo-class is used to define a special state of an element.

For example, it can be used to:

- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus

We have worked with some of these during our [CSS Links and Lists Lesson](https://redi-school.github.io/nrw-html-and-css-2021-spring/lesson10/)
The most important pseudo classes which this section covers are:

- `:first-child`
- `:last-child`
- `:nth-child()`

If times allow it we would cover some additional pseudo classes.

# 4. CSS Pseudo Elements

Apart from pseudo classes there are also pseudo elements which can be styled with a certain CSS Pseudo Elements Selectors. A CSS pseudo-element is used to style specified parts of an element. For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

The most important Pseudo Elements we would cover are:

- `::first-line`
- `::first-letter`
- `::before`
- `::after`
- `::selection`

# 5. CSS Attribute Selectors

It is possible to style HTML elements that have specific attributes or attribute values. This section covers how to do that.

# Glossary & Terminology

- `Pseudo-class` - A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s). For example, `:hover` can be used to change a button's color when the user's pointer hovers over it.
- `Pseudo-element` - A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). For example, `::first-line` can be used to change the font of the first line of a paragraph.

# Homework

- Look in your project and review CSS selectors. Think about cases where you can use a different CSS Selector version so that you decrease the number of CSS rules you use and make your CSS file more structured and maintainable.
- In [Checkpoint 20](https://github.com/ReDI-School/nrw-html-and-css-2021-spring/tree/checkpoint18), we have changed some CSS rules definition to show you how different selectors can make more sense in some cases. Please take inspiration from it for your personal project.

# Resources

- [Attribute Selectors](https://www.w3schools.com/css/css_attribute_selectors.asp)
- [Categorization of CSS Selectors](https://www.w3schools.com/css/css_selectors.asp)
- [Combinator Selectors](https://www.w3schools.com/css/css_combinators.asp)
- [Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp)
- [Pseudo-elements](https://www.w3schools.com/css/css_pseudo_elements.asp)
