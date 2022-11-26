---
title: Lesson 13 - Selectors, Cascade, Specificity and Inheritance
nav_order: 13
---

# Cascade, Specificity, Inheritance, and Advanced Selectors

In this class, we want to improve our understanding of how CSS applies the styles we write on the HTML elements.

We will also learn various CSS Selectors which are not so often used but still important. The theory would be accompanied with practical examples for each selector case.

Students should be able to understand situations like: what happens when there are conflicting rules, and what happens if multiple selectors are attempting to add a style to an element.

Note: Teachers are not limited to the examples shown in this note.

## Class Agenda

- Precedence
- Specificity
- Inheritance
- Selectors
- !important

## Introduction

The word "Cascading" in Cascading Style Sheets is a key concept to understand. As your webpage styles increases, you may have a situation where a particular CSS rule you just wrote is not applying to the element because another rule is taking Precedence, or because of a specificity case. We explore these concepts below.

## Precedence

When multiple CSS rules are used on an element at the same specificity level, CSS needs to decide which rule to apply to the element. When this situation happens, the rule that comes last in the source code will be used. Examples:

```css
/* Example 1 */
/* If you have multiple places in your stylesheet(s) where the background is
defined for the h1 tag like below, the pink background will be applied
because it comes last. */

h1 {
  background: red;
}

h1 {
  background: pink;
}
```

```css
/* Example 2 */
/* If you have an h1 with two classes like this:
<h1 class="heading top-heading">Heading</h1>, and you applied the same
css rule with the different classes as shown below, the last one that 
comes last in the source code will be used (i.e padding: 0)
*/
.heading {
  padding: 50px;
}

.top-heading {
  padding: 0;
}
```

## Specificity

Specificity is how CSS decides which rule to apply when there are multiple rules targeting an element using different selectors or source location (e.g inline style, element selector, class selector, id selector).

Different types of selectors have different specificities. For example, an ID selector has a higher specificity than a Class selector, while a Class selector has higher specificity than an Element selector. In this section, we want to show (with examples) how different selector rules are ranked and which ones win over the others.

```css
/* Consider an example with a heading like this
  <h1 class="heading" id="main-h1">Heading</h1>,
  which color will be applied on the page?
*/
.heading {
  color: pink;
}

#main-h1 {
  color: blue;
}
```

### Inline Styles

If you use the HTML **style** attribute to apply styles to an element, that style will override any other styles defined in a `<style>` tag or a stylesheet.

Example:

Consider a heading like this:

```html
<h1 class="heading" id="main-h1" style="color: red">Heading</h1>
```

```css
/*
 The color rule (red) defined in the style attribute will always win over
 other color values defined using CSS selectors
*/
.heading {
  color: pink;
}

#main-h1 {
  color: blue;
}
```

## Selectors

### 1. CSS Selectors Recap

We have written a decent amount of CSS rules for our website so far. While the amount of CSS rules is high, we have not used too many different CSS Selectors for our rules. We have mainly used the Simple CSS Selectors such as

- the CSS element Selector
- the CSS id Selector
- the CSS class Selector
- the CSS universal Selector
- and others

### 2. CSS Combinator Selectors

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

- descendant selector (space)
- child selector (>)
- adjacent sibling selector (+)
- general sibling selector (~)

### 3. CSS Pseudo-classes

A pseudo-class is used to define a special state of an element.

For example, it can be used to:

- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus

We have worked with some of these during our [CSS Links and Lists Lesson](https://redi-school.github.io/berlin-html-and-css/lesson9/)
The most important pseudo-classes which this section covers are:

- `:first-child`
- `:last-child`
- `:nth-child()`

If times allow it we would cover some additional pseudo-classes.

### 4. CSS Pseudo Elements

Apart from pseudo-classes there are also pseudo-elements which can be styled with a certain CSS Pseudo-elements Selectors. A CSS pseudo-element is used to style specified parts of an element. For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

The most important Pseudo-elements we would cover are:

- `::first-line`
- `::first-letter`
- `::before`
- `::after`
- `::selection`

### 5. CSS Attribute Selectors

It is possible to style HTML elements that have specific attributes or attribute values. This section covers how to do that.

## Inheritance

Inheritance is another crucial part of CSS Cascade. Inheritance is how some CSS rules, which are set on parent elements, are inherited by their child elements. In this section, we want to show examples where a property value (e.g color, font-family) is inherited by an element.

Example:

```html
<section>
  <p>This is the first paragraph in the section</p>
  <p class="note">
    This is another paragraph with <span>a span element</span> inside it
  </p>
</section>
```

```css
/* the two paragraphs inherits sans-serif font-family,
 but only the first one applies it, because the second paragraph
 has a font-family set on it. The span inherits cursive font from
 the second paragraph
 */
section {
  font-family: sans-serif;
}

.note {
  font-family: cursive;
}
```

## !important

This is a special declaration in CSS that you can use to overrule all the specificity or inheritance logic explained above. When you apply `!important` to a rule, it becomes the most specific one and overrides the normal rules of the cascade. It also overrides inline styles in the markup.

It is useful to know that `!important` exists, however, you are strongly advised not to use it unless if you absolutely need to.

## Extra Exercise

- Show how to see overridden rules using the Dev Tools. [Example](https://developer.chrome.com/docs/devtools/css/overrides/)

## Glossary & Terminology

- `Inheritance` is a process of receiving values of properties by a child element from its parent element.
- `Specificity` determines which CSS rule is applied by the browsers.
- `Pseudo-class` - A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s). For example, `:hover` can be used to change a button's color when the user's pointer hovers over it.
- `Pseudo-element` - A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). For example, `::first-line` can be used to change the font of the first line of a paragraph.

## Homework

- Look in your project and review CSS selectors. Think about cases where you can use a different CSS Selector version so that you decrease the number of CSS rules you use and make your CSS file more structured and maintainable.
- Practice your selector skills with this game: ["CSS Diner - the fun way to practice selectors"](http://cssdiner.com). Share a screenshot of your completed levels in the Classroom channel.

## Resources

- [Calculating CSS Specificity Value](https://css-tricks.com/specifics-on-css-specificity/#calculating-css-specificity-value)
- [MDN Cascade and Inheritance Page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)
- [MDN Specificity](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)
- [Precedence in CSS](https://css-tricks.com/precedence-css-order-css-matters/)
- [Attribute Selectors](https://www.w3schools.com/css/css_attribute_selectors.asp)
- [Categorization of CSS Selectors](https://www.w3schools.com/css/css_selectors.asp)
- [Combinator Selectors](https://www.w3schools.com/css/css_combinators.asp)
- [Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp)
- [Pseudo-elements](https://www.w3schools.com/css/css_pseudo_elements.asp)
