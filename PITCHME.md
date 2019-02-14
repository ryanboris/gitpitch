## Imperative

```js
function nSquared(arr) {
  for (let i = 0; i < arr.length; i = i + 1) {
    Math.pow(arr[i], 2)
  }
  return arr
}
```

@snap[text-06]
@ul[spaced text-black]

- Beginning with the number 0, represented by i
- Locate the item at index 0 of the array, arr[0]
- Square that item using the Math.pow method
- Increase the value of i by +1
- Locate the item at index 1 of the array, arr[1]
- Square that item using the Math.pow method
- ... repeat until ...
- Locate the item at that is at the index which is 1 less than the array length
- Square that item using Math.pow method
- Stop the loop according to the upper bound instruction
- return the array
  @snapend

---

## Declarative

```js
function nSquared(arr) {
  return arr.map(i => Math.pow(arr[i], 2))
}
```

@snap[text-06]
@ul[spaced text-black]

- Take the array and return a new array with each item squared.
  @snapend

---

# Imperative

```js
const btn = document.getElementById('btn')
btn.addEventListener('click', function() {
  btn.classList.includes('toggle')
    ? btn.classList.remove('toggle')
    : btn.classList.add('toggle')
})
```

@snap[text-06]
@ul[spaced text-black]

- Get the btn element by its ID and set that reference equal to the variable `btn`
- Listen for a click on the `btn` element
- When the btn element is clicked execute the anonymous callback function by:
  - first checking to see if the btn element's classlist contains a class by the name of `toggle`
  - if it does then remove the toggle class from the btn element
  - if it doesn't then add the toggle class to the btn element
  - await for the next click event to happen and when it does execute the callback and continue as described above
    @snapend

---

# Declarative

```html
<Btn onClick={this.toggle}>Click me!</Btn>
```

@snap[text-06]
@ul

- Execute the `toggle` function when the Btn component is clicked.
  @snapend
