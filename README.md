# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Mobile version](https://github.com/Kitty10206/frontend-mentor/blob/nft-preview-card/NFT%20preview%20card%20component%20mobile.html.png?raw=true)
![Desktop version](https://github.com/Kitty10206/frontend-mentor/blob/nft-preview-card/NFT%20preview%20card%20component%20desktop.html.png?raw=true)


### Links

- Solution URL: [On Codepen](https://codepen.io/HannahWillis/pen/GRxXdpa)


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- CSS float
- Mobile-first workflow


### What I learned

This took me about 2-3 hours to complete.

```html
<svg id="viewimage" width="48" height="48" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path d="M0 0h48v48H0z"/><path d="M24 9C14 9 5.46 15.22 2 24c3.46 8.78 12 15 22 15 10.01 0 18.54-6.22 22-15-3.46-8.78-11.99-15-22-15Zm0 25c-5.52 0-10-4.48-10-10s4.48-10 10-10 10 4.48 10 10-4.48 10-10 10Zm0-16c-3.31 0-6 2.69-6 6s2.69 6 6 6 6-2.69 6-6-2.69-6-6-6Z" fill="#FFF" fill-rule="nonzero"/></g></svg>
```
I learned how to use svg files and manipulate them.

```css
#viewimage {
  transition: 1s ease;
  opacity: 0;
  position: absolute;
  top: 32%;
  left: 50%;
  transform: translate(-50%, -50%); /*I copied this from w3schools and it made the image centered*/
  -ms-transform: translate(-50%, -50%);
  cursor: pointer;
  background-color: hsla(178, 100%, 50%, 0.5);
  padding: 108px;
  border-radius: 10px;
}
#viewimage:hover {
  opacity: 1;
}
```
I found the transform: translate from W3schools, which fixed the image being off-center. As my card was not changing size when I switched to desktop (by design), I fixed the size of the overlay image. I learned how to use :hover styles to change the opacity of an object, which was very exciting.

```css
.card { ...
  box-shadow: 
    10px 30px 50px #0C1729, 
    -10px 30px 50px #0C1729, 
    40px -30px 50px hsla(217.24, 54.72%, 10.39%, 0.6), 
    -40px -30px 50px hsla(217.24, 54.72%, 10.39%, 0.6), 
    40px 55px 50px hsla(217.24, 54.72%,	10.39%, 0.6), 
    -40px 55px 50px hsla(217.24, 54.72%, 10.39%, 0.6);
}
```
Here I made the shadow larger. There is a way to do this in one line, but for clarity's sake I separated them all.

### Continued development

I have still not managed to get GitHub to work. I tried building this in a different editor, not codepen, but I think I prefer codepen. I switched the code to codepen for display.

### Useful resources

- [Mozilla docs and Entheos web](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)(https://www.entheosweb.com/tutorials/css/multiple_shadows.asp#:~:text=Multiple%20shadows%20can%20be%20made,offset%20and%20y%2Doffset%20values.) - These helped me design the shadows like in the example, where the shadow is larger than the box and not offset.
- [In motion hosting](https://www.inmotionhosting.com/support/website/website-design/align-float-images-css/) I referred to this again on floating images, which I used for the profile picture at the bottom.
- [W3 docs](https://www.w3docs.com/snippets/css/how-to-style-a-horizontal-line.html) I re-learned how to style a horizontal line using this resource.


## Author

- Codepen - [Hannah Willis](https://codepen.io/HannahWillis)
- Frontend Mentor - [@Kitty10206](https://www.frontendmentor.io/profile/Kitty10206)