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



## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![./Screenshot.png](./Screenshot.png)


### Links

- Solution URL: [https://github.com/MaxiJRom/Product-preview-card-component](https://github.com/MaxiJRom/Product-preview-card-component)
- Live Site URL: [https://maxijrom.github.io/Product-preview-card-component/](https://maxijrom.github.io/Product-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- media queries

### What I learned

Si el border-radius no está funcionando, la mejor solucion es darle overflow:hidden a la caja contenedora.

Usar la etiqueta "picture" en el HTML te permite colocar dos imagenes en un mismo lugar y elegir cuál de las dos mostrar de acuerdo al width de la pantalla. Con este función se ahorra código en el stylesheet.
  
Si se define un cambio estético del border durante el :hover, debe entonces definirse también cómo será su border ANTES del :hover, de otra forma el navegador le colocará un borde negro por default.

```html

        <picture class="card__imagen">
        <source media="(min-width: 501px)" class="card__imagen" srcset="./images/image-product-desktop.jpg">
        <img src="./images/image-product-mobile.jpg" alt="imagen producto" class="card__imagen">
      </picture>
  
  
```
```css

  
.card__boton {
    background-color: var(--clr-dark-cyan);
    text-align: center;
    padding: 0.6em;
    border-radius: 0.6em;
    border: 2px outset #fff;
}

.card__boton:hover,
.card__boton:focus {
    cursor: pointer;
    border: 2px inset #fff;
  
  
```
- Frontend Mentor - [@MaxiJRom](https://www.frontendmentor.io/profile/MaxiJRom)
