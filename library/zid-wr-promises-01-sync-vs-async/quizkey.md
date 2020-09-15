**Promises: Sync vs Async Code**

1. What will be logged and in what order?

```javascript
console.log(1);

setTimeout(() => {
  console.log(2);
}, 100);

setTimeout(() => {
  console.log(3);
}, 0);

console.log(4);
```

**Answer:  D** 1, 4, 3, 2


2.  What will be logged and in what order?

```javascript
console.log(1);

setTimeout(() => {
  console.log(2);
}, 0);

setTimeout(() => {
  console.log(3);
}, 0);

console.log(4);
```

**Answer: C** 1, 4, 2, 3
