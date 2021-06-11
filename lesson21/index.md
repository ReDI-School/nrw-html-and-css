---
title: Lesson 21 - CSS Background & Color Values
nav_order: 21
---

# CSS Background & Color Values

In previous classes, we applied flat fill colors (e.g `red`, `#ccc`) as backgrounds on elements,
but CSS gives up a lot more options and effects that we can apply on backgrounds.

In this lesson, we will look at other effects that CSS allows us to apply on element backgrounds.

## Class Agenda

1. Recap
1. Background Images
1. Background Gradients
1. Opacity
1. blend-mode
1. Gradient generator
1. Other CSS Color Values

## 1. Recap

We have used `background: green`. The `background` property is a shorthand property that is capable of setting
[the color, image, size and other properties](https://developer.mozilla.org/en-US/docs/Web/CSS/background#constituent_properties).

So, when we write `background: green`, it is similar to writing `background-color: green`.

## 2. Background Images

The `background-image` property is used to apply a graphic (e.g JPG) or gradient to the background of an element.
The url() keyword lets you provide the location of the image. You can also use the shorthand `background` property.
See different examples below:

```css
.celebrate {
  background-image: url(balloons.jpg);
}

body {
  background: url(sweet_texture.jpg);
}

.section {
  background: no-repeat url("../../media/examples/lizard.png");
}
.fancy {
  /* You can also set multiple images */
  background-image: url("sparkles.png"), url("balloons.jpg");
}
```

## 3. Background Gradients

You can also use CSS to create a gradient with different colors and apply that as a background image.
There are different types of gradients, e.g. radial, linear, repeating. They are shown with examples below.

```css
div {
  background: radial-gradient(black, red);
}
p {
  background: linear-gradient(45deg, black, transparent);
}
.comic {
  background-image: conic-gradient(#ff8, #e71);
}
.gradient {
  background-image: repeating-linear-gradient(
    45deg,
    #af002d,
    #131417 10px,
    #373c49 10px,
    #6d2ee5 20px
  );
}
```

## 4. Opacity


6. CSS Gradient generator (https://html-css-js.com/css/generator/)
   (maybe 60min)

7. Other CSS Color Values (HEX, RGB (RGBA), HSL)
   Color keywords (currentcolor, inherit, transparent)
   (40min)

# Homework

Read More about:

- CSS Outline https://www.w3schools.com/css/css_outline.asp
- CSS Border-Image https://www.w3schools.com/css/css3_border_images.asp
- CSS Box-Shadow

# Resources

- [Repeating Gradients Background](https://www.youtube.com/watch?v=muE2B0Zylbw)
- [MDN background property page](https://developer.mozilla.org/en-US/docs/Web/CSS/background)
- [A Complete Guide to CSS Gradients](https://css-tricks.com/a-complete-guide-to-css-gradients/)
