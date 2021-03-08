**JavaScript foundations: Scope**

1.  Evaluate the following code. What will be logged or what error will first be thrown?

```javascript
const colors = ["blue", "green", "red", "yellow"];
for (let i = 0; i < colors.length; i++) {
  colors[i] = colors[i].toUpperCase();
}
console.log(i);
```
**Answer: D**
`Uncaught ReferenceError: i is not defined`

2.Evaluate the following code. What will be logged or what error will first be thrown?

```javascript
const colors = ["blue", "green", "red", "yellow"];
for (const i = 0; i < colors.length; i++) {
  colors[i] = colors[i].toUpperCase();
}
console.log(i);
```
**Answer: F**
`Uncaught TypeError: Assignment to constant variable`

3. Evaluate the following code. What will be logged or what error will first be thrown?

```javascript
const favoriteColorCount = {
  blue: 8,
  green: 6,
  red: 3,
  yellow: 1,
};

const favoriteColor = "";
const maxCount = 0;
for (let color in favoriteColorCount) {
  const count = favoriteColorCount[color];
  if (maxCount < count) {
    maxCount = count;
    favoriteColor = color;
  }
}

console.log(favoriteColor);
```
**Answer: E**
`Uncaught TypeError: Assignment to constant variable`


4.  Evaluate the following code. What will be logged or what error will first be thrown?

```javascript
const favoriteColorCount = {
  blue: 8,
  green: 6,
  red: 3,
  yellow: 1,
};

let favoriteColor = "";
let maxCount = 0;
for (let color in favoriteColorCount) {
  const count = favoriteColorCount[color];
  if (maxCount < count) {
    maxCount = count;
    favoriteColor = color;
  }
}

console.log(favoriteColor);
```

**Answer: A**
`blue`
