# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Link](#link)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued study](#continued-study)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

- Build out the project to the designs provided

### Link

[Profile card component](https://erinchocolate4.netlify.app/)

## My process

### Built with

- Sass
- BEM
- Flexbox
- CSS Grid

### What I learned

How to use BEM naming convention:

BEM stands for Blocks, Elements and Modifiers.

```html
<div class="card">
    <div class="card__img">
```

I use Sass to write css for the first time:

- I set up Live Sass Complier extension on VS code
- I use nesting and variable in my Sass file

```scss
$dark-cyan:hsl(185, 75%, 39%);
$dark-desaturated-blue:hsl(229, 23%, 23%);
.card__stats {
  display: grid;
  grid-template-columns: 1fr 2fr 2fr 2fr 1fr;

  &__box {
    display: grid;
    place-items: center;
  }
}
```

### Continued study

- Media query and mobile first 

### Useful resources

- [Why I use the BEM naming convention for my CSS](https://www.youtube.com/watch?v=SLjHSVwXYq4)/[You Probably Need BEM CSS in Your Life (Tutorial)](https://www.youtube.com/watch?v=er1JEDuPbZQ) - These videos helped me understand what BEM is and why I need to use it
- [Sass Crash Course](https://www.youtube.com/watch?v=nu5mdN2JIwM&t=1229s) - This videos teaches me how to set up Sass in VS code 
- [5 Sass features that make it better than vanilla CSS](https://www.youtube.com/watch?v=g1kF45K-q7o&t=1415s) - This video and [Sass document](https://sass-lang.com/guide) helped me understand the benefits of using Sass
