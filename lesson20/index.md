---
title: Lesson 20 - CSS Animations & Transitions
nav_order: 20
---

# CSS Animations & Transitions

## Agenda

1. Introduction
2. CSS Transitions
3. CSS Animations
4. CSS transform property


## 1. Introduction

An animation lets an element gradually change from one style to another.
You can create nice animations with CSS on properties such as `color`, `background-color`, `height`, or `width`. On websites they can be used to draw user’s attention, (e.g. showing that a button is clickable or a loading animation)
Animations should not be overused, but can be powerful if used in correct places. 

Some cool examples of animations with CSS:
- https://codepen.io/ste-vg/pen/wdBRZN
- https://codepen.io/pmk/pen/ByXOOq 
- https://codepen.io/Catagen/pen/PqYdXR 
- https://codepen.io/ste-vg/pen/GRooLza 


here are 2 common types to do animations with CSS:

1. CSS Transitions → usually used, when a user interacts with an element
2. CSS Animations → no need for user-interaction to trigger the animation and is more customizable than transitions.

In this lesson, we get to know both animation types.


## 2. CSS Transitions

Transitions are typically applied when a user interacts with an element (e.g when a user hovers or clicks on an element).

To create a transition effect, you must:
- add the `transition` CSS property to the element you want to add an effect to
- specify which CSS property should be added a transition effect to
- specify the duration of the effect (if not specified, the duration is set to 0 second and thereby no animation will occur)
- add the change of the specified CSS property on user interaction (e.g. hover)


### CSS properties
The following are the necessary CSS properties to achieve an animation effect with CSS transitions:

- `transition-property`: used to define what property, or properties, you want to apply a transition effect to. You can also use the keyword `all` to transition all properties possible to transition on the element (usually not recommended)
- `transition-duration`: used to define the duration of a specified transition.
- `transition-delay`: used to define a length of time to delay the start of a transition
- `transition-timing-function`: used to define a function that describes how a transition will proceed over its duration

- `transition`: shorthand for `transition-property`, `transition-duration`, `transition-timing-function` and `transition-delay`

### Example

```css
div {
  transition:  background-color 0.5s ease;
  background-color: red;
}

div:hover {
  background-color: green;
}
```


[EXAMPLE CODEPEN FOR CSS TRANSATIONS](https://codepen.io/redi-school/pen/rNQBwPV)


### Exercise
[Codepen exercise](https://codepen.io/redi-school/pen/gOQYxOd)





## 3. CSS Animations

Animations with CSS animations can start immediately when the page loads, but can also be triggered on interaction of the user. Generally CSS Animations give you more control than CSS transitions. You can customize the animation steps until the end of the animation. Also animations set with CSS animtions can run indefinitely, while CSS transitions only run on user-interaction.

To create an animation effect, you must specify:
- The `animation-name` and steps with the `@keyframes` syntax
- Apply the created animation to a specific CSS selector with the `animation-name`
- Set the duration of the animation

### CSS properties

To create this, we need to know about the `animation` property (plus other related properties) and the `@keyframes` rule.

- `animation-name`: Specifies the name of the `@keyframes` rule describing the animation.
- `animation-duration`: Sets the length of time that the animation should take.
- `animation-delay`: Sets a time before the animation starts
- `animation-iteration-count`: Sets the number of times the animation should run (if it should run indefinetly, then set it to `infinite`)
- `animation-timing-function`: Configures the timing or speed of the animation.

Each keyframe rule defines what should happen at specific moments during the animation.
For example, 0% is the start and 100% is the end,


### Example
```css
.element {
  height: 200px;
  /* animation-name must match @keyframes value */
  animation-name: pulse;
  animation-duration: 5s;
  animation-iteration-count: infinite;
}

/* @keyframes <animation-name> with <percentage> steps */
@keyframes pulse {
  0% {
    background-color: yellow;
  }
  50% {
    background-color: hotpink;
  }
  100% {
    background-color: yellow;
  }
}
```

You can also use keywords `from` and `to` with @keyframes.

```css
h1 {
  font-size: 20px;
  animation-name: size-increase;
  animation-duration: 5s;
}

@keyframes size-increase {
  from {
    font-size: 20px;
  }
  to {
    font-size: 80px;
  }
}
```

[EXAMPLE CODEPEN FOR CSS TRANSATIONS](https://codepen.io/redi-school/pen/eYQORBa)


### Exercise
[Codepen exercise](https://codepen.io/redi-school/pen/BaGBZPP)


## 4. CSS Transform property

The `transform` property is usually used alongside animations. It allows you to visually manipulate an element by skewing, rotating, translating, or scaling. You can set transform on an element without animations e.g

```css
div {
  width: 20px;
  height: 20px;
  transform: scale(20);
}
```

but works well with transitions and animations e.g

```css
a {
  font-size: 2em;
  transition: transform 0.3s ease-out;
  display: inline-block;
}

a:hover {
  /* this lifts up the link on hover */
  transform: translate(0, -5px);
}
```

# Homework

Finish the exercises for CSS Transitions and CSS Animations and continue working on your final project.



# Resources

- [The slides of the course](https://docs.google.com/presentation/d/1PWFMZvMdZsPoXnNrIQFNV_KB3imKB2qPSfrmZBZBvZk)
- [Animation on MDN Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
- [Transition property](https://css-tricks.com/almanac/properties/t/transition/)
- `Animatable CSS properties` - List of CSS properties can be animated using CSS Animations or CSS Transitions. More info [here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties).
- [Difference between CSS Animations and CSS Transitions](https://blog.hubspot.com/website/css-transition-vs-animation )
- [Solution CSS Transitions Exercise](https://codepen.io/redi-school/pen/yLRWyKj)
- [Solution CSS Animations Exercise](https://codepen.io/redi-school/pen/NWEKgaB)
