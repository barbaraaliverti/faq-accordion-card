# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![image](https://user-images.githubusercontent.com/64551613/121228984-cbb6bb80-c863-11eb-8882-5bd17026597d.png)

### Links

- [Solution URL](https://faq-accordion-card-umber-five.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- SASS
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This was my first project from [Front End Mentor](https://www.frontendmentor.io/) and I chose what I thought would be a pretty simple one, but I ended up learning so much from it! 

First, I realized I didn't know how to deal properly with SVG, so I had to study how to manipulate them - how to insert them in my code, how to resize them and how to overlap them.  I chose to use CSS grid to overlap the images and I was very happy ewith the result.

Another challenge was to make the accordion Q&A using only CSS. I ended up using checkboxes and although I like the result, I couln't find a way to leave only one answer open at the time. I could've done it with radio buttons, but them I wouldn't be able to hide the answers when clicking on the arrows.

```css
  //hide answers
    .accordion-content {
        color: $text-neutral-dark;        
        max-height: 0px;
        overflow: hidden;
        transition: all .25s ease-in-out;
    }

    //show answers
    .toggle:checked + .lbl-toggle + .accordion-content {
        padding-bottom: 1rem;
        max-height: 3rem;
    }
```
Finally, it was my first time using SASS in a project and I loved it :) So much easier to organize the styling. 


### Continued development

I wanted to make only one answer visible at a time, but I couldn't find a way to achieve this using CSS only. I might do some extra digging later or finally add some JS to fix this and make the accordion prettier. 

### Useful resources

- [Scaling SVG on CSS Tricks](https://css-tricks.com/scale-svg/) and [How to use SVG (in portuguese) from Willian Justen](https://willianjusten.com.br/como-usar-svg/)- These helped me to understand how to scale my SVG!
- [How to overlap images in CSS on Bricampgomez](https://bricampgomez.com/blog/how-to-overlap-images-in-css/) - Interesting way to overlap images using CSS grid.
- [How to create a responsive SVG (in portuguese) from Willian Justen](https://willianjusten.com.br/criando-svg-responsivo/) - This article helped me to understand how to make my svg responsive (although I ended up using two different image compositions for desktop and mobile)
- [Checkbox hack](https://css-tricks.com/the-checkbox-hack/#faq-answer-revealing) - this is where I got the checkbox hack from to build reaveling answers :) very interesting!

## Author

- [Portfolio](https://barbaraaliverti.github.io/)
- [LinkedIn](https://www.linkedin.com/in/barbaraaliverti)