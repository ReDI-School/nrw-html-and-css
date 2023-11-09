---
title: Lesson 16 - CSS Media Queries
nav_order: 16
---

# CSS Media Queries

## 1. Introduction

Media queries are a fundamental aspect of creating responsive web designs, which allow websites to adapt to different devices and screen sizes.

In this lesson, we'll explore how media queries work and how you can use them to create layouts that look great on both desktop and mobile devices.

While desktop computers were once the primary way people connected to the internet, the rise of smartphones has dramatically changed the game. Today, most people use their smartphones to access the internet. Mobile internet usage has surpassed desktop usage in recent years, and this trend is only expected to continue.

Your job, as a web developer, is to develop websites that work seamlessly across a variety of devices, including smartphones and tablets. We’re going to look at a concept called Media Queries, which will help us to do this.

## 2. Using Media Queries

A media query is a conditional statement that checks certain conditions (such as screen size, device orientation, or aspect ratio) and applies a set of CSS styles based on those conditions.

For example, a media query could apply different font sizes or layout styles to a website when viewed on a smartphone device versus a laptop.

Media queries work by using the "@media" rule in CSS, which specifies a set of styles to apply when certain conditions are met.

Developers can use a variety of conditions to trigger a media query, such as "max-width", "min-width", "orientation", and "device-pixel-ratio".

## 3. Syntax

```css
@media screen and (min-width: 768px) {
  body {
    font-size: 20px;
  }
}
```

## 4. Example

[CSS Media Queries Demo](https://codepen.io/redi-school/pen/QWZaeJP)

## 5. The viewport tag

The viewport HTML meta tag is important for accurate media queries because it helps the browser determine the size of the viewport (the visible area of the webpage).
Some mobile devices and other narrow screens render pages in a virtual window or viewport, which is usually wider than the screen, and then shrink the rendered result down so it can all be seen at once.

<meta name="viewport" content="width=device-width, initial-scale=1" />

Without this tag, the browser may use a default viewport size, which can cause media queries to work incorrectly.

## 6. Exercise

Start a new project in your IDE. you’ll need at least one HTML file, and a CSS file. For your HTML, create a simple page layout. For example:

A title section with some links
3-4 sections containing text and images

Next use some Media queries to make some changes across different breakpoints.

If making a whole page responsive feels overwhelming, try just laying out some divs with different sizes and colours, and set those to different values in your media queries. Once you’re comfortable with that, try building a basic page layout (header with links, a section or two, a footer) then make them responsive!

# Glossary & Terminology

- `CSS at-rule` - An instruction that ‘tells’ css how to behave. For example, @media instructs the CSS that it should only apply the media queries content if the device meets the criteria of the condition/s.
- `media type` - Describes the device category, for example screen, print, or all.
- `media feature` - Describe specific characteristics of the device, such as min-width or max-width.

# Homework

Continue to practice using Media Queries.

# Resources

- [Using Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
- [What is Mobile First Design](https://medium.com/@Vincentxia77/what-is-mobile-first-design-why-its-important-how-to-make-it-7d3cf2e29d00)

# Slides

<iframe src="https://docs.google.com/presentation/d/1AkNMFqZrDZrenNuzXGQh9Q7X3MzhXScbCTQnyApRgLQ/embed" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
