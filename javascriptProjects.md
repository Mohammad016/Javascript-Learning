# *Chai Aur Code* JavaScript Project code solution

## Project Link
[Chai Aur Code JS Project](https://stackblitz.com/edit/dom-project-chaiaurcode?file=index.html)

## Project-1

```javascript
const buttons = document.querySelectorAll('.button')
const body = document.querySelector('body')

buttons.forEach(function(button) {
    button.addEventListener('click', function(e){
        body.style.backgroundColor = e.target.id;
    });
});
```

## Project-2

```Javascript

```