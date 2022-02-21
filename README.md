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
- [Author](#author)


## Overview

Here is my second Frontend Mentor project. A NFT preview card component which contain NFT image, title, description, value, time remaining and information about creator. I have used HTML5 and SCSS to build this project.


### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)


### Links

<!-- - Solution URL: [Add solution URL here](https://your-solution-url.com) -->
- Live Site URL: [https://shamilussainc.github.io/NFT-preview-card-component/](https://shamilussainc.github.io/NFT-preview-card-component/)

## My process

- Developed html body structure
- Started building with mobile first approach
- Used SCSS to create css files
- Used Grid and Flexbox for element alignment
- Implemented hover states


### Built with

- Semantic HTML5 markup
- SCSS
- CSS
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

In this project i have learned to add hover state effects on a image. where i stacked 2 images ie, NFI image and a View icon image. The View icon image will only be visible when NFI image in hover state.

```html
	<div class="img-container">
		<img class="equilibrium" src="./images/image-equilibrium.jpg" alt="Image Equilibrium">
		<img class="view" src="./images/icon-view.svg" alt="View Icon">
	</div>
```
```css
main .img-container {
  line-height: 0;
  border-radius: 10px;
  position: relative;
  -webkit-transition: .5s;
  transition: .5s;
}

main .img-container .equilibrium {
  width: 100%;
  border-radius: inherit;
  -webkit-transition: .5s;
  transition: .5s;
}

main .img-container .view {
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
  -webkit-transition: .5s;
  transition: .5s;
}

main .img-container:hover {
  background-color: var(--cyan);
  cursor: pointer;
}

main .img-container:hover .equilibrium {
  opacity: .5;
}

main .img-container:hover .view {
  opacity: 1;
}
```

## Author

- Linkedin - [Shamil ussain c](https://www.linkedin.com/in/shamil-ussain-c-893282187/)
- Frontend Mentor - [@shamilussainc](https://www.frontendmentor.io/profile/shamilussainc)
- Twitter - [@c_ussain](https://twitter.com/c_ussain)
