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
               
3 - Consider the diagram of a part of the DOM below. Which snippet of HTML is most likely to generate this DOM structure?

![image.png](http://res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/9995e67b60d2933540dce4c7e06662d9-image.png)

A. 
```
<div>
  <h1>A DOM question</h1>
  <div>
    <h2>A second heading</h2>
     <p>Another paragraph</p>
     <img src="me.jpg"/>
  </div>
  <p>This is a paragraph of text</p>
</div>
```
B.
```
<div>
  <h1>A DOM question</h1>
  <div>
    <h2>A second heading</h2>
     <p>Another paragraph</p>
     <img src="me.jpg"/>
  </div>
  <p>This is a paragraph of text</p>
</div>
```
C.
```
<div>
  <h1>A DOM question</h1>
     <div></div>
     <p>This is a paragraph of text</p>
</div>
    <h2>A second heading</h2>
     <p>Another paragraph</p>
     <img src="me.jpg"/>
```
D.
```
    <div>First div</div>
     <h1>A DOM question</h1>
     <div>Second div</div>
     <p>This is a paragraph of text</p>
    <h2>A second heading</h2>
     <p>Another paragraph</p>
     <img src="me.jpg"/>
```

**Correct Answer: A** 


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

B. A CSS property describes the general category or type of stylistic change that you'd like to make

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

11 - Which of the following methods returns the first element that matches a CSS selector?

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

13 - What is the difference between Git and GitHub?

A. Git is the open-source system used for version control. GitHub is the company that runs a website where users can store and manage versions of their code projects online.

B. Git is a project's folder that contains all of the files for the project, as well as each file's revision history. GitHub is the open-source system used for version control.

C. Git and Github are the same thing.

D. Git is the open-source system used for version control.GitHub is the person who creates a repo and therefore determines if it is public or private.

**Correct Answer: A**

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
