**Javascript on your machine: Environment variables & script arguments**

1. Which of the following is the correct way to write an environment variable?

**Answer:  D** `TERM_PROGRAM_VERSION`

2. Assume you run the following file with this command: `node file.js fact`. What will be shown in the terminal?

```javascript
let argument = process.argv[1];
if (argument) {
  if (argument === "fact") {
    console.log(
      "Here is a fun plant fact: Most plant life is found in the ocean!"
    );
  } else {
    console.log("Sorry, I did not understand that command.");
  }
} else {
  console.log("You need to enter a command!");
}
```

**Answer:  B** `"Sorry, I did not understand that command."`

3. Assume you run the following file with this command: `node file.js`. What will be shown in the terminal?

```javascript
let argument = process.argv[2];
if (argument) {
  if (argument === "fact") {
    console.log(
      "Here is a fun plant fact: Most plant life is found in the ocean!"
    );
  } else {
    console.log("Sorry, I did not understand that command.");
  }
} else {
  console.log("You need to enter a command!");
}
```

**Answer:  C** `"You need to enter a command!"`

4. Assume you have access to an environment variable called `USER` which points to the value `Robin`. 

Then, assume you run the following file with this command: `node file.js Nice to meet you` . What will be shown in the terminal?

```javascript
console.log(process.env.USER + " says: " + process.argv[2]);
```

**Answer:  A** `"Robin says: Nice"`




