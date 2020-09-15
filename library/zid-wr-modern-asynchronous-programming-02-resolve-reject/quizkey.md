**Modern Asynchronous Programming: Resolve & Reject**

1.  What will be logged from the following promise chain?

```javascript
Promise.resolve(10)
  .then((value) => Promise.reject(value - 1))
  .then((result) => console.log("Success:", result))
  .catch((result) => console.log("Failure:", result));
```

**Answer:  D** `Failure: 9`

2.  What will be logged from the following promise chain?

```javascript
Promise.resolve({ name: "Orion" })
  .then((value) => {
    return value.meaning
      ? Promise.reject(value)
      : Promise.resolve({ error: "Missing key." });
  })
  .then((result) => console.log("Success:", result))
  .catch((result) => console.log("Failure:", result));

```

**Answer:  B** `Success:  { error: "Missing key." }`
