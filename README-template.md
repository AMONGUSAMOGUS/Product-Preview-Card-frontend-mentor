# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![file:///C:/Users/ENG%20Eldeeb/Desktop/first%20course/Capture.PNG](mobile)
file:///C:/Users/ENG%20Eldeeb/Desktop/first%20course/Capture1.PNG (desktop)
file:///C:/Users/ENG%20Eldeeb/Desktop/first%20course/Capture3.PNG (active)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL:
/*html code*/
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <link rel="stylesheet" href="styles.css">
  <title>Frontend Mentor | Product preview card component</title>
<link href='https://fonts.googleapis.com/css?family=Fraunces' rel='stylesheet'>
<link href='https://fonts.googleapis.com/css?family=Montserrat' rel='stylesheet'>
</head>
<body>
<div class="container">
<div class="preview"?
<article>
<picture>
<source media="(min-width:600px)" srcset="file:///C:/Users/ENG%20Eldeeb/Downloads/product-preview-card-component-main/product-preview-card-component-main/images/image-product-desktop.jpg">
    <img src="file:///C:/Users/ENG%20Eldeeb/Downloads/product-preview-card-component-main/product-preview-card-component-main/images/image-product-mobile.jpg" alt="picture of perfume" id="image">
</picture>
</article>
</div>
  <div class="text">
  <h2 class="info1">PERFUME</h2>

  <h1 class="info1">Gabrielle Essence Eau De Parfum</h1>

  <p class="info1">A floral, solar and voluptuous interpretation composed by <br>Olivier Polge,
  Perfumer-Creator for the House of CHANEL.</p>

  <ul id="price" class="info1">
    <li id="paf">$149.99</li>
  <li id="pbe">$169.99</li>
</ul>
  <button class="btn"><pre><svg width="15" height="16" xmlns="http://www.w3.org/2000/svg"><path d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z" fill="#FFF"/></svg>   <span>Add to Cart</span></pre></button>
</div>
</div>
<div class="attribution">
  Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
  Coded by <a href="https://www.frontendmentor.io/home">Bakr</a>.
</div>
</body>
</html>
/*css code*/
body {
  background-color: hsl(30, 38%, 92%);
  margin:0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  display:flex;
  width:40%;
  margin:9em auto;
overflow: hidden;
  border-radius: 10px;
}
.attribution { font-size: 11px; text-align: center; }
.attribution a { color: hsl(228, 45%, 44%); }
.preview {
  width:50%;
}
#image {
  width:100%;
  height:auto;
}
.text {
  width:50%;
  background-color: white;
  display:flex;
  flex-direction: column;
padding-left: 1.5em;
}
#price {
  display:flex;
  list-style-type: none;
  margin-left: -2.5em;
  margin-top: 1em;

}
#paf {
  color:hsl(158, 36%, 37%);
  font-size:2rem;
  font-weight:700;
}
#pbe {
  color:grey;
  margin-top:0.5em;
  margin-left:0.5em;
  text-decoration: line-through;
}
.btn {

  background-color:hsl(158, 36%, 37%);
  color:white;
  width:90%;
  margin-top:2em;
  border-radius: 10px;
  border:0;

}
span{
  font-family: "Montserrat";
  font-weight: 700;
}
svg {
  vertical-align: text-bottom;
}
h2 {
font-family: "Montserrat";
color:hsl(228, 12%, 48%);
}

h1{
margin-top:-0.5em;
font-family: "Fraunces",sans-serif;
font-weight: 700;
}

p {
font-size: 14px;
font-weight: 500;
margin-top:-0.5em;
font-family: "Montserrat";
color:hsl(228, 12%, 48%);
}
ul {
margin-top:-0.5em;
font-family: "Fraunces",sans-serif;
font-weight: 700;
}
.btn:active {
background-color: #1a4031;
cursor: pointer;
}
@media screen and (max-width:375px) {
  .container{
    display:flex;
    flex-direction: column;
    width:95%;
margin:1em auto;
  }
  .preview {
    width:100%;
  }
  .text{
    width:100%;
  }
  .btn {
    margin-top: -1em;
    margin-bottom: 1em;
  }
}

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
-google fonts

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned
<article>
<picture>
<source media="(min-width:600px)" srcset="file:///C:/Users/ENG%20Eldeeb/Downloads/product-preview-card-component-main/product-preview-card-component-main/images/image-product-desktop.jpg">
    <img src="file:///C:/Users/ENG%20Eldeeb/Downloads/product-preview-card-component-main/product-preview-card-component-main/images/image-product-mobile.jpg" alt="picture of perfume" id="image">
</picture>
</article>
/*This code helped me with the image changing from desktop to mobile image as the device width changes*/

### Continued development

I want to focus on CSS Layout and positioning properties I feel lost in this topic but other than than I am happy with my progress so far.

### Useful resources

## Author


- Frontend Mentor - [@whenimechainthesuma](https://www.frontendmentor.io/profile/whenimechainthesuma)




## Acknowledgments

Thanks for stackoverflow anonymous user who gave me the solution to "the image changing from desktop to mobile image as the device width changes" dilemma.
