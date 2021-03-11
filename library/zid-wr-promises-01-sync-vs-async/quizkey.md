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

**Answer: D** 1, 4, 3, 2

**Explanation** `console.log(1);` and `console.log(4);` are synchronous functions and execute immediately.

`setTimeout()` is an asynchronous function, so each call adds an event to the event queue. The first `setTimeout()` call waits 100 milliseconds before executing while the second `setTimeout()` call waits 0 milliseconds. As a result of the additional wait time, `console.log(2);` is printed _after_ `console.log(3);`.

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

**Explanation** `console.log(1);` and `console.log(4);` are synchronous functions and execute immediately.

`setTimeout()` is an asynchronous function, so each call adds an event to the event queue. In this case, both `setTimeout()` calls wait 0 milliseconds. Because the wait time is zero for both, the callbacks are executed in the order they were added to the event queue. As a result, `console.log(2);` is printed _before_ `console.log(3);`.
