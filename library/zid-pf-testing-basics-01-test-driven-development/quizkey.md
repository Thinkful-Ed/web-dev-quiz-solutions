**Testing: Test driven development**

1.  Assume you are about to write a function called `getTopScorerName()` with the following functionality.

```javascript
const students = [
  { name: "Ray Morales", score: 10.0 },
  { name: "Li Harvey", score: 9.8 },
  { name: "Ellie King", score: 8.4 },
];

getTopScorerName(students); //> "Ray Morales"
getTopScorerName([]); //> null
```

Select all of the following possible cases you _could_ test.

**Answer: All of the above**

2. Assume you are about to write tests for the `getTopScorerName()` function.

Which of the following tests would be the _first_ you might write if you were following a test driven development process.

**Answer: D** That the `getTopScorerName()` function exists and is a function.