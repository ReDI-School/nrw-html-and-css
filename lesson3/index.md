---
title: Lesson 3 - HTML Building Blocks
nav_order: 3
---

# HTML Building Blocks

## Class Agenda

* Elements
* Whitespace
* Comments
* Combining elements
* Pens
* Quiz
* Homework

## Elements

HTML documents consist of a set of elements. In order to define elements and how they relate to each other, we mark up text content using tags.

### Anatomy of a typical HTML element

A simple HTML element - in this case a paragraph - looks like this:

```html
  <p>Text contents</p>
```

#### Opening tag

The part `<p>` is the **opening tag**. it gives the browser information about the element's type, in this case `p`, which represents a paragraph, surrounded by angle brackets (`<` and `>`). We also use the term "tag name" for `p` in this case. The browser will consider everything following the opening tag up to the point where it finds a closing tag (of the matching type/name) to be the element's content.

#### Content

The **content** of an element is everything between its opening and closing tag. The content can consist of text, other HTML elements or nothing at all. In our example, the content is `Text contents`.

An empty element - in this case a table cell - could look like this:

```html
<td></td>
```

#### Closing tag

Just like the opening tag, the **closing tag** also contains the type of the element. It is written with an additional `/`. In our first example, our closing tag is `</p>`, because our element is of the type `p`, representing a paragraph.

#### Attributes

While closing tags always look the same, opening tags can contain extra information in the form of **attributes**.

```html
<p class="my-class">Text contents</p>
<a href="https://www.redi-school.org">To the ReDI Website</a>
```

You can put as many attributes into an opening tag as you like.

```html
<a href="https://www.redi-school.org" class="featured-link" title="Click me!">To the ReDI Website</a>
```

Some attributes don't even need a value, but are complete as a single word.

```html
<p hidden>The browser will not display this element.</p>
```

### Anatomy of a void element

A void element is special type of element that must not contain anything. No text, no HTML elements. This is why a void element also **must not** have a closing tag.

The following code inserts three different void elements:

```html
<hr>
<br>
<img src="dog.jpeg">
```

Never do this:

```html
<hr></hr>
<br></br>
<img src="dog.jpeg"></img>
```

You might encounter void elements that contain a trailing `/`, e.g.

```html
<br />
<hr/>
```

Some developers prefer to write void elements like this, so they're easier to recognize. In modern HTML, any opening tag can contain a trailing `/`, which will just be ignored by the browser.

## Whitespace

You might think that space characters, line breaks and tabs in HTML are displayed in an unexpected way. The following two code examples are equivalent:

```html
<p>HTML is so much fun!</p>
```

```html
    <p   >       HTML   
  is  so     

        
      much
  fun!
</p>
```

Generally, the browser will interpret every number of so-called **whitespace** characters (spaces, tabs or line breaks) as one single space character, as long as it's greater than 0.

This is why whitespace is perfect for formatting, i.e. making our code more readable. Instead of just something like...

```html
<ul><li>Lorem</li><li>Ipsum</li><li>Dolor</li></ul>
```

...we can make our code nice and readable:

```html
<ul>
  <li>Lorem</li>
  <li>Ipsum</li>
  <li>Dolor</li>
</ul>
```

## Comments

**Comments** are parts of the code that are always ignored by the browser. There are numerous reasons why you as a developer might want to use them, with the most common ones being:

* Explaining your code to your future self or other developers
* Increasing the readability of your code
* Temporarily deactivating some of your code

Comments are not HTML elements, although they look quite similar:

```html
<!-- This is a comment -->
<p>This sentence contains five <!-- and not eight --> words</p>
<p>This is one <!-- </p>
<p> --> single paragraph</p>
```

## Combining elements

Elements can't only contain text contents, but also other elements. Actually, every HTML page is just one single element (of the type `html`) that contains other elements. For now, we'll keep things simple and will concentrate on the visible parts of a document.

When an element contains another element, the **child element** is **nested** within its **parent element**.

```html
<div><!-- opening tag of the parent element -->

  Some text content of the parent element.

  <div><!-- opening tag of the child element -->
    Contents of the child element.
  </div><!-- closing tag of the child element -->

  More text content of the parent element.

</div><!-- closing tag of the parent element -->
```

In this case, the content of the parent element consists of three lines of text (including the child element's content).

When a child element is surrounded by a parent element, you could also say it is wrapped in it.

When you structure your document, you can nest elements infinitely and put them next to each other almost any way you like.

```html
<header>
  <nav>
    <ul>
      <li>
        <a href="home.html">
          Home
        </a>
      <li>
      <li>
        <a href="contact.html">
          Contact
        </a>
      </li>
      <!-- ... -->
    </ul>
  </nav>
  <input type="text" placeholder="Search...">
</header>
<main>
  <article><!-- ... --></article>
  <article><!-- ... --></article>
  <!-- ... -->
</main>
```

## Pens

* [Simple HTML elements: Find and fix all mistakes](https://codepen.io/redi-school/pen/VwGVVNJ) ([Solution](https://codepen.io/redi-school/pen/xxaQoWz))
* [Wheel of Fortune](https://codepen.io/redi-school/pen/VwGVqKw)
* [Updating a simple blog page](https://codepen.io/redi-school/pen/ZEMmVmw) ([Solution](https://codepen.io/redi-school/pen/mdGQNmP))
* [Comments](https://codepen.io/redi-school/pen/QWVJPjM) ([Solution](https://codepen.io/redi-school/pen/rNZQXRg))

Bonus Pens we didn't cover:
* [Bold and italic text in one line](https://codepen.io/redi-school/pen/MWqzxdO)
* [Line breaks - inline vs. block elements](https://codepen.io/redi-school/pen/oNPQOwN)

## Quiz

* [Quiz 1](https://create.kahoot.it/share/html-css-lesson-3-short-warm-up-quiz/fe0f52ca-e48b-42fe-aa46-bfd6e1963839) / [live](https://kahoot.it/?pin=2630819&refer_method=link)
* [Quiz 2](https://create.kahoot.it/share/html-css-lesson-3-quiz-on-the-building-blocks-of-html/a432307c-be9b-472b-abc0-42d04751ffb2) / [live](https://kahoot.it/?pin=9441788&refer_method=link)

## Homework

[You can find today's homework on CodePen: "Hi!"](https://codepen.io/redi-school/pen/JjaexdX)

Assignment:
1. Format the code, so you can get a better idea of its structure
2. Try to display your initials (or two letters of your choice)