# Frontend Mentor - Insure landing page solution

This is a solution to the [Insure landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/insure-landing-page-uTU68JV8). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS 
- Desktop-first workflow

### What I learned

The major challange of this project is adding backgrounds of the containers which demands to use the psuedo elements before and after the container. And it was very nice and challenging project for using the before and after psuedo elements. I will highly recommend this project to do the exercise of psuedo elements. After the psuedo element in this project flex is also required that gives you the challenge to use css flexboxes. 
And when we come to the javascript, we see that here is a toggle button which shows and closes the hammburger menu.

To see how you can add code snippets, see below:

```css

h1::before{
    content: "";
    height: 1px;
    width:150px;
    background-color: white;
    position: absolute;
    top: 0;
    left: 0;
}

header::after{
    content: "";
    background: url(./images/bg-pattern-intro-right-desktop.svg);
    background-repeat: no-repeat;
    background-position: top right;
    width: 50%;
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;
    z-index:2;
}
```
```js
const hamburger = document.getElementById('hamburger');
const menu = document.getElementById('menu');

hamburger.addEventListener('click', () => {
    hamburger.classList.toggle('show');
    menu.classList.toggle('show');
});
```


### Continued development

There are some techniques which was very useful, like the concept of keeping the elements in a flexbox and container two different divs. The toggle menu was a bit challenging part and i want to be more flexible with this so i will use these concepts on coming projects. 


### Useful resources

- [Youtube](https://www.youtube.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [w3schools](https://www.w3schools.com) - This is an amazing article which helped me finally understand all the concepts of flexbox and toggle. I'd recommend it to anyone still learning this concept.


## Author

- Website - [Durgesh kumar rai](https://www.your-site.com)
- Frontend Mentor - [@durgeshrai633](https://www.frontendmentor.io/profile/durgeshrai633)
