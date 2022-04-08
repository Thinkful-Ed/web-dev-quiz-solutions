### Frontend Development: HTML, CSS and JavaScript evaluation (quiz 2)


1 - Choose the correct statement(s).

A. JavaScript is used for adding interactivity to web pages.

B. HTML creates the structure of a web page

C. HTML applies styling to a web page

D. CSS applies styling to a web page

**Correct Answer: A, B, & D**



2 - You would like all h2 headings nested within `<section>` containers to have a font-size of 35px. Which of the following CSS selector would you apply?
  
A. section > h2 { font-size: 35px };

B. section h2 { font-size: 35px };
  
C. section.h2 { font-size: 35px };
  
D. section < h2 { font-size: 35px };

**Correct Answer: B**
               
3 - Which of the following statements are true about the DOM?

A. The DOM stands for Document Object Model.

B. It provides a way to update the content, structure and style of an HTML document.
`
C. It defines the properties of all HTML elements, and the methods to access them.

D.None of the above


**Correct Answer: A, B and C** 


4 - True/False. The following HTML code is correctly written:
```html
<main>
  <h1>Welcome to Thinkful<h1>
  <p>This is a simple paragraph created within HTML.<p>
</main>
```

A. True

B. False

**Correct Answer: B**



5 - Which of the following statement(s) are TRUE about CSS?

A. A CSS declaration consists of the property and value applied to the selector

B. A CSS property describes the general category or type of stylistic change that you'd like to make to an HTML element.

C. A CSS selector identifies the HTML element that should be affected by the CSS declaration

**Correct Answer: A, B, & C**


6 - Evaluate the following code. What will be logged, or what error will first be thrown?

```js
const favoriteColorCount = {
  blue: 8,
  green: 6,
  red: 3,
  yellow: 1,
};

let favoriteColor = "";
let maxCount = 0;
for (let color in favoriteColorCount) {
  const count = favoriteColorCount[color];
  if (maxCount < count) {
    maxCount = count;
    favoriteColor = color;
  }
}

console.log(favoriteColor);
```

A. blue

B. undefined

C. Uncaught ReferenceError: favoriteColor is not defined

D. Uncaught SyntaxError: Identifier 'count' has already been declared

E. Uncaught TypeError: Assignment to constant variable

**Correct Answer: A**


7 - What is a unit test?

A. A manual process for testing an application's workflow from beginning to end

B. An automated piece of code that tests whether many separate parts of a software work together as a group

C. A manual process that involves human testers working from a detailed test script

D. An automated piece of code that checks the behavior of an individual part of a program

**Correct Answer: D**


8 - What is the correct value of the array holidays after the following code executes?

```js
let holidays = [];
holidays.push("Martin Luther King Jr. Day")
holidays[1] = "Valentine's Day";
holidays.push("President's Day")
```

A. ["Valentine's Day", "President's Day"]

B. ["Martin Luther King Jr. Day", "President's Day"]

C. ["President's Day"]

D. ["Martin Luther King Jr. Day", "Valentine's Day", "President's Day"]

**Correct Answer: D**


9 - What will be output to the console after the code runs?
```js
let total = 10;
let amount = "10";

if(total === amount){
  console.log('Same')
}else if(total == amount){
  console.log('Similar')
}else if(total = amount){
  console.log('This is incorrect. Remember a single equals sign is for assignment, not for comparisons.')
}
```

A. Same

B. Similar

C. This is incorrect. Remember, a single equals sign is for assignment, not for comparisons.

**Correct Answer: B**


10 - What will print to the console when the following code executes?
```js
let totals = [10,20,30,40];
for(let i=3; i >= 0; i--){
  console.log(totals[i])
}
```

A.
```
10
20
30
40
```
B.
```
40
30
20
```
C.
```
40
30
20
10
```
D.
```
30
20
10
```

**Correct Answer: C**

11 - Which of the following DOM methods returns the first element that matches a CSS selector?

A. querySelectorAll()

B. querySelector()

C. classList()

D. getElements()

**Correct Answer: B**

12 - What are the keys in the album object?
```js
let album = {
  "name" : "My Favorite Things",
  "author" : "Coltrane"
}
```

A. "name" and "author"

B. "My Favorite Things" and "Coltrane"

C. "name" and "author", "My Favorite Things" and "Coltrane"

**Correct Answer: A**

13 - In Git, which of the following commands allows you to commit the changes that you made?

A. git commit -add-all

B. git add -commit

C. git commit -add -all

D. git commit -m <commit message>

**Correct Answer: D**

14 - In Git, which of the following commands will change files from untracked to staged?

A. git init

B. git add -A

C. git push origin main

D. git commit -m <commit message>

**Correct Answer: B**

15 - Which of the following commands will initialize a Git repository in a folder?

A. git remote -v

B. git init

C. git add -A

D. git pull origin main

E. git push origin main

F. git commit -m <commit message>

**Correct Answer: B**

16 - Which of the following commands allows you to send  the commits from your local branch in your local Git repository to a remote repository

A. git remote -v

B. git init

C. git add -A

D. git pull origin main

E. git push origin main

F. git commit -m <commit message>

**Correct Answer: E**
