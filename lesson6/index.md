---
title: Lesson 6 - Units of Measurement in HTML & CSS; Formatting Text with CSS; CSS Basic Colors
nav_order: 6
---

# CSS Text Formatting

## Class Agenda

1. Welcome & icebreaker (15min)
2. Units of Measurement in HTML & CSS (5min)
3. CSS Comments
4. Formatting Text with CSS (5min)
5. CSS Fonts (10min)
6. CSS Basic Colors (Borders & Backgrounds) (5min)
   Total: 40min

## 1. IceBreaker

## 2. Units of Measurement in HTML & CSS

We measure most distances in centimeters, or cm. On a computer, the most common unit for measuring distances is _pixels_, or px.

You have already used this a few times, such as setting an image to have `width: 400px;`. You can set the size of text this way as well, such as `font-size: 20px;`.

Another common way to resize elements using CSS is with _percentage sizing_ with the `%` symbol. This is most common when setting the width of elements.

Elements sized with a percent are sized _relative to their parent elements_. For example, if you have a box that is `400px` wide and you place an image in it, and you set the image width to be `50%`, the image will be `200px` wide.

Here is the HTML for that example:

```html
<div>
  <img
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7b/M%C3%BCnster%2C_Observantenkirche_--_2021_--_9112.jpg/2560px-M%C3%BCnster%2C_Observantenkirche_--_2021_--_9112.jpg"
  />
</div>
```

And here is the CSS:

```css
div {
  width: 400px;
}

img {
  width: 50%;
}
```

There are several other CSS units that you may see and use (see the [Resources](#resources) section below for more), but these two are the most common. You can create complex and beautiful layouts just using `px` and `%`!

## 3. CSS Comments

Just like we can add HTML comments to our html files we can also add CSS comments to our CSS code. This section will cover how to do that.

## 4. Formatting Text with CSS

We have learned how to apply basic text formatting on a website by using some [HTML text formatting tags](https://redi-school.github.io/berlin-html-and-css/lesson4/#3-html-text-styling-tags). However, most of the text formatting is done via abundant CSS text formatting rules. Therefore, this section will cover some of those CSS rules including:

- Text Alignment (`text-align`)
- Text Decoration

There are another sections that you can check in the respective resources:

- Text Direction
- Text Indentation
- Text-Shadow

## 5. CSS Fonts

A crucial role on all websites plays the font. It can give a totally different look and feel on your website.

This section will cover:

- Font-families
- Font-style [`font-style`](https://www.w3schools.com/css/css_font_style.asp)

## 6. CSS Basic Colors

This section will cover some basic CSS colors [standard color names](https://www.w3schools.com/colors/colors_names.asp) (e.g. Tomato, Azure, DodgerBlue, etc.). It will also practice the usage of those color names together with the following CSS Rules, which students will learn:

- Background Color
- Text Color
- Border Color (keep in mind that this only covers the border color without the border style and sizes. We can use `2px solid` without going into details)

# Exercise Description

1. Practice using CSS styles with this [codepen](https://codepen.io/redi-school/pen/bGxywzN)

2. Create your own personal biography page, including:

- multiple different headings,
- multiple paragraphs (you can use lorem\*5 to quickly fill with placeholder text)
- lists,
- images
  Ad CSS styles to your page. Try to use everything we learned today!

---

# Homework

1. Keep working in your personal biography page until it has all of the following elements, attributes, selectors, and styles:

- HTML elements: h1, h2, h3, p, img, ul, ol, li, a
- HTML attributes: class, id, src, href
- CSS selectors: type (h1, h2, p, etc.), class (.), id (#), selector list (like h1, p {...})
- CSS styles: color, font-size, font-family, background-color, border, padding, margin

If part of this feels repetitive, that’s because it is! Repetition helps us remember material and get faster at accessing it in our brains. Practice is your bestfriend.

- Read more about different web font families [here](https://www.hostinger.com/tutorials/best-html-web-fonts). Get to know what the different companies are using
- Make sure to use your own image / photo on your websites
- (Optional) Try CSS diner [CSS Diner](https://flukeout.github.io/). See if you can complete the first 12 levels!
- (Optional) Check out the nice [CSS tricks](https://css-tricks.com/almanac/properties/t/text-shadow/) with text shadow

# Resources

- [Recap of HTML Tree](http://web.simmons.edu/~grabiner/comm244/weekfour/document-tree.html)
- [CSS values and units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)
- [CSS Basic Colors](https://www.w3schools.com/css/css_colors.asp)
- [CSS Standard Names](https://www.w3schools.com/colors/colors_names.asp)
- [CSS Text](https://www.w3schools.com/css/css_text.asp)
- [CSS Font](https://www.w3schools.com/css/css_font.asp)
- [Web Safe Fonts](https://www.w3schools.com/css/css_font_websafe.asp)

# Slides

<iframe src="https://docs.google.com/presentation/d/10OmFwXbrmZFZ1n65YscQxQPJL4lfeH40EF2beaJr5Kg/edit" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
