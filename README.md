# Frontend Mentor - Grid landing page solution

This is a solution to the [Grid landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/grid-landing-page). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)




## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- Open and close the navigation menu at any screen size (optional JavaScript)



### Links

- Solution URL: [Add solution URL here]((http://127.0.0.1:5500/SkosanaPhumii-gridLandingPage/index.html))
- Live Site URL: [Add live site URL here]((https://phumiiskosana.github.io/SkosanaPhumii-gridLandingPage/))

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- CSS Grid
- Desktop-first workflow
- CSS Animations
- CSS prefers-reduced-motion 
- [Styled Components](https://styled-components.com/) - For styles
- 



### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<div class="grid">
        <!-- Hero -->
        <div id="hero">
          <h1>A classroom for every child.</h1>

          <p>We fund the schools, train the teachers, and measure what works — so every child we reach today becomes a graduate tomorrow.</p>
        </div>
        <!-- Stats -->
        
          
        <section id="students">
          <div class="statistics"> ...
**Instead of creating 2 div elements to make a desktop and mobile grid layout work, as I did before, I used one grid div element, which I am proud of.**

<details class="menu-panel">
        <summary><img class="menu-img" src="menu.png" alt="bridge collective menu image"/>
          <img class="menu-close-img" src="close.png" alt="bridge collective menu image"/>
        
        </summary>
**Learning about details and summary elements and seeing them work in my code was thrilling. The details element creates a widget which discloses additional information, like a menu or navigation, on a web page until the widget is toggled open. The summary element, which is the first child of the details element, holds the name or image that labels the disclosure widget, which in my case is a menu image when the widget has not been opened, and a close image when the widget is opened.
```

```css
details[open] .menu-img{
        display: none;
    }
details[open] .menu-close-img{
        display: inline-block;
    }
**This shows what will be visible when the details element is opened by clicking the first child of the summary element, which is the menu icon; then only the close icon will be visible when the details element is open. **

details[open] .menu{
        animation-name: slide-in;
        animation-duration: 0.5s;
    }
    @keyframes slide-in {
        from{
            translate: 80vw 0;
            scale:40% 1;
        }
        to{
            translate:80vw 0;
            scale: 40% 1;
        }
    }
**Using animations to slide in the menu as the details element is being opened.

@media (prefers-reduced-motion: reduce){
    details[open] .menu{
        animation-name: slide-in;
        animation-duration: 0.2s;
    }
**Allowing people who prefer no motion or have it reduced to obtain that with ease.


```



### Continued development

Continuing to do challenges like these and not stopping because I cannot use a specific coding language yet, but finding other ways to make a web page interactive. I will learn more HTML5 elements and capabilities as well as CSS3 limitations, and use every tool I can access.

### Useful resources

- [W3Schools](https://www.w3schools.com/) - This helped me find a 3-column grid layout with a 4x4 grid, ending up with a 5 grid layout.
- [MDN](developer.mozilla.org) - This helped me with understanding the use of many elements and properties when I built my code. I'd recommend it to anyone still learning this concept.



### AI Collaboration

Describe how you used AI tools (if any) during this project. This helps demonstrate your ability to work effectively with AI assistants.

- I used both Google Gemini and Microsoft Copilot
- I used them to find out how to use both HTML and CSS to open and close a menu, how to blend an image into the page background, as well as for debugging.
-Some images did not blend well, which meant I had to change their backgrounds manually. 



## Author


- Frontend Mentor - [@phumiiskosana](https://www.frontendmentor.io/profile/phumiiskosana)




