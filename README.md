# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot_desktop.png)
![](./screenshot_mobile.png)

### Links

- Solution URL: [on Frontend Mentor](https://www.frontendmentor.io/solutions/huddle-landing-page-with-a-single-introductory-section-9SmiOGr5el)
- Live Site URL: [on Github](https://pykm.github.io/huddle-landing-page-with-single-introductory/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

To use font icon library - [IcoMoon](https://icomoon.io/) in your css code, you need to do things below:
1. Import the font files into the css.
1. Set general rules, like `font-family`, `color` and  `line-height` for all icons.
1. And in our case, use `padding`, `border` and `border-radius` to adjust the appearance of the social icons.
1. Use different content represent different icons.

To see my added code snippets, see below:

```html
<ul class="social-icons">
  <li class="facebook">
    <a href="#"></a>
  </li>
  <li class="twitter">
    <a href="#"></a>
  </li>
  <li class="instagram">
    <a href="#"></a>
  </li>
</ul>
```
```css
@font-face {
  font-family: 'icomoon';
  src:  url('../fonts/icomoon.eot?rp1lj8');
  src:  url('../fonts/icomoon.eot?rp1lj8#iefix') format('embedded-opentype'),
    url('../fonts/icomoon.ttf?rp1lj8') format('truetype'),
    url('../fonts/icomoon.woff?rp1lj8') format('woff'),
    url('../fonts/icomoon.svg?rp1lj8#icomoon') format('svg');
  font-weight: normal;
  font-style: normal;
  font-display: block;
}

.social-icons a {
  border: 0.05em solid;
  border-radius: 170893px;
  color: var(--default-font-color);
  /* use !important to prevent issues with browser extensions that change fonts */
  font-family: 'icomoon' !important;
  speak: never;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  padding: 0.5em;

  /* Better Font Rendering =========== */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.facebook > a:before {
  content: "\ea90";
}
.twitter > a:before {
  content: "\ea96";
}
.instagram > a:before {
  content: "\ea92";
}
```

### Continued development

Technique that I'm not completely comfortable with, can be found in this challenge:
- Use font icon library.

Technique that I found useful, although not using in this challenge:
- SASS

### Useful resources

- [IcoMoon App](https://icomoon.io/app/#/select) - This made me able to use Icon Font in my project to represent social icons.

## Author

- Website - [PYkm](https://pykm.github.io/)
- Frontend Mentor - [@PYkm](https://www.frontendmentor.io/profile/PYkm)
