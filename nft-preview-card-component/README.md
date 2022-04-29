# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). 

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
- See hover states for interactive elements

### Screenshot

![screenshot](https://github.com/erinchocolate/frontend-mentor-challenge/blob/master/nft-preview-card-component/screenshot.png)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Using CSS custom properties (variables)

```css
:root {
  --main-bg-color: hsl(217, 54%, 11%);
  --card-bg-color: hsl(216, 50%, 16%);
  --line-color: hsl(215, 32%, 27%);
  --soft-blue:hsl(215, 51%, 70%);
  --cyan:hsl(178, 100%, 50%);
  --hover-cyan:hsl(178, 100%, 50%, 0.5);
  --white:hsl(0, 0%, 100%);
}
```

How to add hover effect and color overlay on the image:

![hover-effect](https://github.com/erinchocolate/frontend-mentor-challenge/blob/master/nft-preview-card-component/hover.png)

```css
.image__overlay{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: var(--hover-cyan);
  opacity: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: opacity 0.25s;
  border-radius: 8px;
}

.image__overlay:hover{
  cursor: pointer;
  opacity: 1;
}
```

### Useful resources

[Image Hover Text Overlay Effect with HTML & CSS - Web Design Tutorial](https://www.youtube.com/watch?v=exb2ab72Xhs) - I learned how to make overlay hover effect from this vide

[A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This guide helps me understand how to align items using Flexbox



