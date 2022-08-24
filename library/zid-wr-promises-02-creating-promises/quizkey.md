## Promises: Creating promises

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

    **Answer:** A: `"Your fortune is: null"`

    **Explanation:** `setTimeout()` is an asynchronous function, which means the code inside the `setTimeout()` callback will _always_ run _after_ the code in the current file. As a result, `fortune` has not been set to a value by the time ``console.log(`Your fortune is: ${fortune}`);`` is called.

2. What will be the state of the promise below after 1,000 milliseconds?

    ```javascript
    const promise = new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve("Completed!");
      }, 100);
    });
    ```

    **Answer:** B. fulfilled

    **Explanation:** Calling the `resolve()` function always causes a pending promise to become fulfilled.

3. What will be the state of the promise below after 1,000 milliseconds?

    ```javascript
    const promise = new Promise((resolve, reject) => {
      console.log("Completed!");
    });
    ```

    **Answer:** A. pending

    **Explanation:** A promise will remain in the pending state indefinitely, until either `resolve()` or `reject()` is called.
    
4. True/False. A promise is an object that wraps asynchronous code and provides methods that let you extract a single result from that code.

    **Answer:** A. True
