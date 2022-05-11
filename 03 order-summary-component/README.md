# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Link](#link)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Link

[Order summary card](https://app.netlify.com/sites/erinchocolate3/overview)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CUBE CSS methodology

### What I learned

The default starting code snippet for CSS:

```css
/* Box sizing rules and remove default margin and padding */
*, *:before, *:after {
  box-sizing: border-box;
}

/* Remove list styles on ul, ol elements with a list role, which suggests default styling will be removed */
ul[role="list"],
ol[role="list"] {
  list-style: none;
}

/* Set core root defaults */
html:focus-within {
  scroll-behavior: smooth;
}

/* A elements that don't have a class get default styles */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Make images easier to work with */
img,
picture {
  max-width: 100%;
  display: block;
}

/* Inherit fonts for inputs and buttons */
input,
button,
textarea,
select {
  font: inherit;
}
```
**CUBE methodology**

CUBE stands for **Composition Utility Block Exception**.

The composition's job is to create layout:

```css
/* composition - layout*/
.grid {
  display: grid;
  row-gap: 1.5rem;
}
```

The utility is just a css class that does one job:

```css
/* utility - styling*/

.margin-48 {
  margin-left: 3rem;
  margin-right: 3rem;
}

.text-large {
  font-size: 1.75rem;
}
```

A block is a card element of button element that has "specific group of rules that only apply in that context":

```css
.button {
  cursor: pointer;
  border: none;
  background-color: var(--clr-more-pale-blue);
  font-size: 0.9rem;
  opacity: 1;
}
```

The exception is "a deviation from the rules outlined in a block".

I add the exception using a data attribute like this:

```html
<button class="button fw-extra-bold br-1" data-type="primary" data-attr="transition">
```

```css
.button[data-type="primary"] {
  color: var(--clr-white);
  background-color: var(--clr-bright-blue);
  padding: 0.8rem;
  box-shadow:0.3rem 0.5rem 0.5rem 0.3rem var(--clr-more-pale-blue);
}
```

### Continued development

I need to learn more Flexbox and Grid to make the plan part look as close to the design

### Useful resources

- [CUBE CSS](https://cube.fyi/#what-does-cube-css-stand-for) - This document helped me understand the basic principle of CUBE.
- [A look at the CUBE CSS methodology in action](https://www.youtube.com/watch?v=NanhQvnvbR8&t=2148s) - This is an amazing video which helped me finally understand CUBE and apply it into this project. 
- [The most common HTML mistake that I see](https://www.youtube.com/watch?v=NexL5_Vdoq8) , [When to Use Semantic HTML Elements Instead of Divs](https://www.youtube.com/watch?v=ZThq93Yuwd0), [How to Write Better HTML and CSS](https://www.youtube.com/watch?v=xE7VOZbHhFY) - These video helped me understand how to structure HTML with Semantic HTML5 
- [Concepts to help simplify CSS layouts](https://www.youtube.com/watch?v=nYyFf-97Qqg&t=12s), [The 6 most important CSS concepts for beginners](https://www.youtube.com/watch?v=JnTPd9G6hoY) - These two videos helps me understand the basic principle of CSS
