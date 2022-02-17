**JavaScript on your machine: Installing packages**


1. Skim the page below:
* [npmjs.com: faker.js](https://www.npmjs.com/package/@faker-js/faker)
Which of the following options most correctly describes the purpose of the `faker` package?

**Answer:  B** The package helps you generate randomized, fake data.

2.  Skim the page below:
* [npmjs.com: chalk](https://www.npmjs.com/package/chalk)

Which of the following options most correctly describes the purpose of the `chalk` package?

**Answer:  C** The package helps you to print text to the terminal in a variety of colors.

3.  Imagine you are using the [chalk](https://www.npmjs.com/package/chalk) package.

Select all of the following options that:
1. Are valid.
2. Will print the color blue, either as the text color or as a background.

**Answer:  B**

```javascript
let chalk = require("chalk");
chalk.blue("False Indigo");
```

**Answer:  C**

```javascript
let chalk = require("chalk");
chalk.bgBlue("Siberian Squill");
```

**Answer:  D**

```javascript
let chalk = require("chalk");
chalk.blue.bgYellow("Blue Mist Shrub");
```

4.  Which of the following commands will correctly install the `mocha` package as a developer dependency?

**Answer:  D** npm install mocha --save-dev
