# Project Title

This is an HTML5 Canvas where you can paint, based on the 30 days Javascript challenge.

## Getting Started

Click your mouse and move it to enjoy a colorful experience =).

## Demo

## [HTML5 Canvas](https://danielgarciaguillen.github.io/html5canvas/)
![HTML5 Canvas](/image/html5canvas.jpg?raw=true "CssClock")


## Learnings

* How to add select class inside another class and add event listener with:

```
const checkboxes = document.querySelectorAll('.inbox input[type="checkbox"]')
checkboxes.forEach(checkbox => checkbox.addEventListener('click', handleCheck));
```
* How to not draw while moving mouse with:
`let isDrawing = false`

* How to stablish an starting point when drawing:
```
let lastX = 0;
let lastY = 0;
```
* Update last position with `[lastX , lastY] =[e.offsetX, e.offsetY];`

## Built With

* Vanilla Javascript
* Css
* Html
