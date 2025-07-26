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
//Check html file structure and then decide which document to understand first
const form = document.querySelector('form');

form.addEventListener('submit', function (e) {
  e.preventDefault();
  const height = parseInt(document.getElementById('height').value);
  //usage of two different fetching of values from DOM
  const weight = parseInt(document.querySelector('#weight').value);

  const result = document.querySelector('#results');

  if (!height || /^1-9/.test(height) || isNaN(height))
    result.innerHTML = 'Please enter correct Height value';
  else if (!weight || /^1-9/.test(weight) || isNaN(weight))
    result.innerHTML = `Please enter correct Weight value ${weight}`;
  else
  {
    const bmiRes = (weight/((height*height)/10000)).toFixed(2);
    result.innerHTML = `<span>Your BMI is ${bmiRes}</span>`;
  }
  
});

```