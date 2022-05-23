# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Links

- Solution URL: 
  - [#1 solution](https://github.com/erinchocolate/frontend-mentor-challenge/tree/master/10%20testimonials-grid-section/%231)
  - [#2 solution](https://github.com/erinchocolate/frontend-mentor-challenge/tree/master/10%20testimonials-grid-section/%232)

- Live Site URL: [Testimonials grid section solution](https://erinchocolate10.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

How to use grid area and why it's useful:

It's very easy to implement media query with grid area

```css
.testimonial-grid {
  display: grid;
  gap: 1.5rem;
  grid-auto-columns: 1fr;
  grid-template-areas:
   'one'
   'two'
   'three'
   'four'
   'five';

  padding-block: 2rem;
  width: min(95%, 70rem);
  margin-inline: auto;
}

.testimonial:nth-child(1) {
  grid-area: one;
}
.testimonial:nth-child(2) {
  grid-area: two;
}
.testimonial:nth-child(3) {
  grid-area: three;
}
.testimonial:nth-child(4) {
  grid-area: four;
}
.testimonial:nth-child(5) {
  grid-area: five;
```
```css
@media screen and (min-width: 33em) {
  .testimonial-grid {
      grid-template-areas:
      "one one"
      "two three"
      "five five"
      "four four";
  }
}

@media screen and (min-width: 38em) {
  .testimonial-grid {
    grid-template-areas:
     'one one'
     'two five'
     'three five'
     'four four';
  }
}
```
