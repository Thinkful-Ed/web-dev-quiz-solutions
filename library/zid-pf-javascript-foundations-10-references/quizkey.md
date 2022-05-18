## JavaScript foundations: References

1. Evaluate the following code. What will be logged?

    ```javascript
    let a = 10;
    let b = a;
    a = 0;
    console.log(b);
    ```

    **Answer:** B. 10

2. Evaluate the following code. What will be logged?

    ```javascript
    let a = 10;
    let b = 20;
    a = b;
    console.log(a);
    ```

    **Answer:** B. 20

3. Evaluate the following code. What will be logged?

    ```javascript
    let a = 10;
    let b = 20;
    a = b;
    b += 10;
    console.log(a);
    ```
    **Answer:** B. 20

4. Evaluate the following code. What will be logged?

    ```javascript
    let a = [10];
    let b = a;
    a = 0;
    console.log(b);
    ```
    **Answer:** D. `[ 10 ]`

5. Evaluate the following code. What will be logged?

    ```javascript
    let a = [10];
    let b = a;
    a.push(20);
    console.log(b);
    ```
    **Answer:** E. `[ 10, 20 ]`

6. Evaluate the following code. What will be logged?

    ```javascript
    let color = { name: "red", hex: "BF3100" };
    let a = { color: color };
    let b = a;
    color.hex = "FF312E";
    console.log(b);
    ```
    **Answer:** B. `{ color: { name: "red", hex: "FF312E" } }`
