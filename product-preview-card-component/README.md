# Product preview card component

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.png)

### Links

- [Live Site URL](https://toanrb.github.io/frontend-challenges/product-preview-card-component)
- [Solution URL](https://github.com/toanrb/frontend-challenges/tree/master/product-preview-card-component)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

- Practicing how to use Flexbox. Using Flexbox to center things.
- Moblie-first approach.
- Responsive design with Flexbox and media query.
- To set `width` or `height` for a `picture` element, you have to target the `img` element inside that `picture` element. Just targeting the `picture` element doesn't work. For example:

```html
<picture>
	<source srcset="images/image-product-desktop.jpg" media="(min-width: 600px)">
	<img src="images/image-product-mobile.jpg" alt="Image of a Gabrielle perfume bottle">
</picture>
```

This works:  

```css
picture img {
	width: 50%;
}
```

This doesn't:  

```css
picture {
	width: 50%;
}
```