## Promises: Resolving promises

1. Assume that the `tell()` function resolves a value if a string is given to it as its only argument and rejects a value if there is no string.

    What will be logged from the following code?

    ```javascript
    const question = "What will the weather be like today?";
    const promise = tell(question);
    promise.catch(() => {
      console.log("Something went wrong...");
    });
    ```

    **Answer:** C. Nothing will be logged.

2. Assume that the `tell()` function resolves a value if a string is given to it as its only argument and rejects a value if there is no string.

    What will be logged from the following code?

    ```javascript
    tell().then(() => {
      console.log("Success!");
    });
    ```

    **Answer:** C. Nothing will be logged.

3. Assume that the `tell()` function resolves a value if a string is given to it as its only argument and rejects a value if there is no string.

    What will be logged from the following code?

    ```javascript
    const question = "What will the weather be like today?";
    const promise = tell(question);
    promise
      .then(() => {
        console.log("Success!");
      })
      .catch(() => {
        console.log("Something went wrong...");
      })
      .then(() => {
        console.log("Done.");
      });
    ```

    **Answer:** C.

    ```
    Success!
    Done.
    ```

4. Assume that the `tell()` function resolves a value if a string is given to it as its only argument and rejects a value if there is no string.

    What will be logged from the following code?

    ```javascript
    const question = "What will the weather be like today?";
    const promise = tell(question).then(() => {
      console.log(question);
    });

    promise.then(() => {
      console.log("Fortune telling complete.");
    });
    ```

    **Answer:** A.

    ```
    What will the weather be like today?
    Fortune telling complete.
    ```
