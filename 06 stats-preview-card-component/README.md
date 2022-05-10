# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot



## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Mobile-first workflow:

- Write HTML document 
- Basic styling on font, color and etc
- Start with the layout on mobile
- Add media query to complete desktop layout

Responsive design

How to make picture change its size when the screen size changes?

```css
.responsive {
  width: 100%;
  height: auto;
}
```

Overlay

How to add color overlay on the image?

```css
.image {
  position: relative;
}

.image:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background: rgba(124, 28, 219, 0.5);
}
```

```html
<div class="card__image image">
      <img class="image--mobile" src="images/image-header-mobile.jpg" alt="women working in the office">
```

### Useful resources

- [Introduction To Responsive Web Design - HTML & CSS Tutorial](https://www.youtube.com/watch?v=srvUrASNj0s) - I learned to add border to each element to help me understand the layout.
