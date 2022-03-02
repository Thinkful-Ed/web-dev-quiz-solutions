1. Take a look at the following function and associated test.

```javascript
const { expect } = require("chai");

function findStudentsByScore(students, score) {
  if (!score) return null;

  const result = [];
  for (let i = 0; i < students.length; i++) {
    const student = students[i];
    if (student.score === score) result.push(student);
  }
  return result;
}

describe("#findStudentsByScore()", () => {
  it("should return an empty array if no score matches", () => {
    const students = [
      { name: "Thomas Wimmer", score: 8.4 },
      { name: "Paula Pregl", score: 9.8 },
      { name: "Maja Renner", score: 7.3 },
    ];
    const actual = findStudentsByScore(students, 10);
    const expected = [];
    expect(actual).to.eql(expected);
  });
});
```

Select the following lines that are _not_ being fully tested.

**Answer:  A** `if (!score) return null;`
**Answer:  B** `if (student.score === score) result.push(student);`


2.  Out of all of the follow facets to focus on with your coverage tool, which is the _most_ important?

**Answer:  B** Branches