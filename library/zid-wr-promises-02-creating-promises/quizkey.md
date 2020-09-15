**Promises: Creating Promises**

1. What will be logged?

```javascript
let fortune = null;

if (!fortune) {
  setTimeout(() => {
    fortune = "A pleasant surprise is waiting for you.";
  });
}

console.log(`Your fortune is: ${fortune}`);
```

**Answer:  A** `"Your fortune is: null"`

2. What will be the state of the promise below after 1000 milliseconds.

```javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve('Completed!');
  }, 100);
});
```

**Answer:  B** fulfilled

3. What will be the state of the promise below after 1000 milliseconds.

```javascript
const promise = new Promise((resolve, reject) => {
  console.log('Completed!');
});
```
**Answer:  A** pending
