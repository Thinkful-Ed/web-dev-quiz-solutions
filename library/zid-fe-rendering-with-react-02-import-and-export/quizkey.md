## Rendering in React: Import and export

1.  Say you have the following two files.

    #### `a.js`
    ```js
    const fruit = "bananas";
    export default fruit;
    export const cost = 10;
    ```
    #### `b.js`
    ```js
    export const pi = 3.14;
    export const e = 2.718;
    ```

    Which of the following are valid import statements for a file in the same directory as `a.js` and `b.js`?


    **Answer:** A, B, E, G, and I.

    A. `import a from "./a";`

    B. `import fruit from "./a";`

    E. `import fruit, { cost } from "./a"`

    G. `import { pi } from "./b";`

    I. `import { pi, e } from "./b";`
