1. Mentally evaluate the following code. What will be printed to the console?

function shortTitle(title) {
  if (!title.includes(":")) return title;

  let result = "";
  for (let i = 0; i < title.length; i++) {
    const character = title[i];
    if (character !== ":") {
      result += character;
    } else {
      break;
    }
  }

  return result;
}

const title = "Bad Omens: The Nice and Accurate Prophecies of Agnes Nutter, Witch";
const shortened = shortTitle(title);
console.log(shortened);

**Answer: C** "Bad Omens"

2.Select all of the following statements that are true about the above question.

**Answer: B** The break keyword stops the for loop from continuing any further.

**Answer: D** Instead of const character = title[i], the function would work properly if let character = title[i] was used.

3.Mentally evaluate the following code. What will be printed to the console?
const authors = [
  {
    name: { first: "Neil", surname: "Gaiman" },
    knighted: false,
  },
];
const author = {
  name: {
    first: "Terry",
    surname: "Pratchett",
  },
};

authors.push(author);
const result = [ authors, author ];
author.knighted = true;
console.log(result);

**Answer: D**
[
  [
    {
      name: { first: "Neil", surname: "Gaiman" },
      knighted: false,
    },
    {
      name: {
        first: "Terry",
        surname: "Pratchett",
        knighted: true,
      },
    },
  ],
  {
    name: {
      first: "Terry",
      surname: "Pratchett",
      knighted: true,
    },
  },
];


4.Select all of the following statements that are true about the above question.

**Answer: A** Placing the authors array into a new array will lead to an array inside of an array.

**Answer: D** The same object that represents author is inside of the authors array and the result array.
