# Project Title

This is an exercise where you can select multiple elements holding shift, based on the 30 days Javascript challenge.

## Getting Started

Hold shift and select as many elements as you want.

## Demo

## [Hold Shift](https://danielgarciaguillen.github.io/holdshift/)
![Hold Shift](/image/holdshift.jpg?raw=true "HoldShift")


## Learnings

* How to select class inside another class and add event listener with:

```
const checkboxes = document.querySelectorAll('.inbox input[type="checkbox"]')
checkboxes.forEach(checkbox => checkbox.addEventListener('click', handleCheck));
```
* How to create logic where loop between the first element selected and the last one while holding shift:
```
let lastChecked;
function handleCheck(e) {
  // Check if they had the shift key down
  // AND check that they are checking it
  let inBetween = false;
  if (e.shiftKey && this.checked) {
    // go ahead and do what we please
    // loop over every single checkbox
    checkboxes.forEach(checkbox => {
      console.log(checkbox);
      if (checkbox === this || checkbox === lastChecked) {
        inBetween = !inBetween;
        console.log('STarting to check them inbetween!');
      }
      if (inBetween) {
        checkbox.checked = true;
      }
    });
  }
  lastChecked = this;
}
```

## Built With

* Vanilla Javascript
* Css
* Html
