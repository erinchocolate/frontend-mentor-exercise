# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). 

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

- Solution URL: [Four card feature section](https://github.com/erinchocolate/frontend-mentor-exercise/tree/master/08%20four-card-feature-section/src)

- Live Site URL: [Four card feature section](https://erinchocolate8.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

How to put an image at the right bottom of the div.

```html
<div class="outer">
	<img src="....">
</div>
```
```css
div.outer { position: relative; }
div.outer img { position: absolute; right: 0; bottom: 0; }
```
