# Frontend Mentor - Product preview card component solution

This is a solution to the Product preview card component challenge on Frontend Mentor (https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshots](#screenshots)
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

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

The design and specifications of the challange were as follows:

- <a href="https://github.com/billybrook/Product-Preview-Project/blob/main/design/mobile-design.jpg" target="_blank">Mobile Design</a>
- <a href="https://github.com/billybrook/Product-Preview-Project/blob/main/design/desktop-design.jpg" target="_blank">Desktop Design</a>
- <a href="https://github.com/billybrook/Product-Preview-Project/blob/main/design/active-states.jpg" target="_blank">Hover State Of Button</a> 
- <a href="https://github.com/billybrook/Product-Preview-Project/blob/main/design/style-guide.md" target="_blank">Style Guide Specifications</a>

### Screenshots of my finished web page

<img src="images/Screenshot-Desktop-Width-1440px.png" width="700px">
A screenshot of the desktop display of the page for a screen width of 1440 pixels as per the design requirements.
<br />
<br />
<br />
<br />
<img src="images/Screenshot-Mobile-Width-375px.png" height="700px">
A screenshot of the mobile display of the page for a screen width of 375 pixels as per the design requirements.


### Links


- Live Site URL: [Add live site URL here](https://astounding-marshmallow-d98efc.netlify.app)

## My process

### Built with

- HTML5 
- CSS 

### What I learned

This is the first project I have attempted to code. I have leaned heavily on <a href="https://www.youtube.com/watch?v=BMOH4zSLTnQ">Thomas Sankara's YouTube tutorial video</a> in order to code this project. As such, I have learnt many things during my attempt at coding this project, a selection of which follows.

Things I've learnt:
- How to import fonts from google
```css
@import url("https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,700&family=Montserrat:wght@500;700&display=swap");
}
```

In order to import custom fonts to format the HTML one can visit <a href="https://fonts.google.com/" target=_blank>fonts.google.com</a>. From here, one can select the required fonts and use the @import rule with the url from the site. The above code imports the Fraunces and Montserrat font into the file. 
<br />
<br />
<br />
- How to center elements
```css
body{
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}
```
The above code was used to center the elements within the body element of my HTML. Those elements being the product image and the article containing the product information which are both contained within my \<div\ class="container"> tag.
<br />
<br />
<br />
 - How to make a grid of two equal coloumns
```css
  .container{
  display: grid;
  grid-template-columns: repeat(2, 1fr)
  }
 ```
 The above code was used to display the image and product information in a grid with two columns of equal size for the desktop display design.
<br />
<br />
<br />
 
- How to customise a button
```html
<button class="btn"><img src="./images/icon-cart.svg" alt="shopping trolley"> Add to Cart</button>
```
The above html added a shopping trolly icon to the button along with the 'Add to Cart' text.
```css
.btn {
  color: hsl(0, 0%, 100%);
  background-color: hsl(158, 36%, 37%);
  border-color: hsl(158, 36%, 37%);
  font-weight: 700;
  font-size: 1rem;
  width: 100%;
  padding: 1rem;
  border-radius: 0.6rem;
  border-style: none;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}
.btn:hover {
  background-color: hsl(158, 37%, 19%);
  }
```
The above code was used to add various styling effects to the button. I have adjusted the font properties and given the background of the button the correct colour according to the design specifications. In order to make the button the correct size I have used padding around the centred text and shopping trolley icon, and have also made the width 100% of the containing article. The border radius property was used to give rounded edges to the button. The 'cursor: pointer' property changes the hover state of the mouse icon to the pointing finger icon. While the '.btn:hover' styling changes the background colour of the button when hovering over it with the mouse.
<br />
<br />
<br />
- How to write a media query
```html
<article class="perfumepic">
      <picture>
        <source media="(min-width:640px)"srcset="./images/image-product-desktop.jpg"> 
    <img src="./images/image-product-mobile.jpg" alt="fancy pants perfume">
   </picture>
    </article>
```
```css
@media (min-width: 640px) {
  .container {...
  }
  .perfumepic img {...
  }
  ...
  }
```
The above html picture tag was used to import two different images; one for the mobile design and one for the desktop design. Using the '@ media' query 
and setting a min-width for the browser window to 640 pixels allowed me to style the webpage for tablets and computer screens-which are typically at least this width.
If the media query is not satisfied then the mobile display of the webpage is shown.



### Useful resources

- [Product Preview Card Component - Frontend Mentor Challenge](https://www.youtube.com/watch?v=BMOH4zSLTnQ) - As mentioned, Thomas Sankara's YouTube tutorial details how to complete this challenge.
- [W3 Schools](https://www.w3schools.com/default.asp) - I was not really familiar with this popular learning resource before attempting this project. I will be using it as reference site going forward



