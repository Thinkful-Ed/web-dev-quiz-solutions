**Rendering in React: Import and Export**

1.  Say we have the following two files.
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


**Answer:  A** `import a from "./a";`

**Answer:  B** `import fruit from "./a";`

**Answer:  E** `import fruit, { cost } from "./a"`

**Answer:  G** `import { pi } from "./b";`

**Answer:  I** `import { pi, e } from "./b";`
