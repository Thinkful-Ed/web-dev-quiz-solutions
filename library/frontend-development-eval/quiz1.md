1. Choose the correct statement(s).

A. CSS creates the structure of a web page

B. HTML creates the structure of a web page

C. HTML applies styling to a web page

D. CSS applies styling to a web page

**Correct Answer: A & B**

2. Which of the following statement(s) are TRUE about web page templates? You may select more than one option.

A. `<!DOCTYPE html>` is a required first line of code that declares a document as an HTML5 web page.

B. The `<head>` part of a HTML document holds meta information about the web page, such as the title and links to external stylesheets.

C. `<meta name="viewport" content="width=device-width" />` is a meta tag that ensures that a web page displays properly across both desktop and mobile devices by setting the width of the web page to follow the screen width of the device the user is viewing.

D. The `<link>` element is used to connect and reference resources on the internet.

**Correct Answer: A, B, C, & D**

3. Consider the diagram of a part of the DOM below. Which snippet of HTML is most likely to generate this DOM structure?
![image.png](http://res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/9995e67b60d2933540dce4c7e06662d9-image.png)

A. 
```
<div>
  <h1>A DOM question</h1>
    <h2>A second heading</h2>
     <p>Another paragraph</p>
     <img src="me.jpg"/>
     <div></div>
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

4. You have a folder containing some HTML, CSS, JavaScript, and image files and you have to link them together so that your web page would display properly.

Here's the folder structure:
```
├── images
│   ├── doggy.png
│   └── kitty.png
├── index.html
├── src
│   └── script.js
└── styles
    └── global.css
```
Choose the` index.html` file that is properly linked to all images, scripts, and stylesheets in the folder.

A. 
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
  <link href="../styles/global.css" rel="stylesheet" type="text/css" />
</head>
<body>
  <img src="images/doggy.png" alt="doggy">
  <img src="images/kitty.png" alt="kitty">
  <script src="src/script.js"></script>
</body>
</html>
```
B.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
  <link href="styles/global.css" rel="stylesheet" type="text/css" />
</head>
<body>
  <img src="images/doggy.png" alt="doggy">
  <img src="images/kitty.png" alt="kitty">
  <script src="src/script.js"></script>
</body>
</html>
```
C.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
  <link href="styles/global.css" rel="stylesheet" type="text/css" />
</head>
<body>
  <img src="images/doggy.png" alt="doggy">
  <img src="images/kitty.png" alt="kitty">
  <script src="../src/script.js"></script>
</body>
</html>
```
D.
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document</title>
  <link href="styles/global.css" rel="stylesheet" type="text/css" />
</head>
<body>
  <img src="../images/doggy.png" alt="doggy">
  <img src="../images/kitty.png" alt="kitty">
  <script src="src/script.js"></script>
</body>
</html>
```
**Correct Answer: B**

5. Select all statements that are TRUE about CSS Style Sheets.

A. Internal style sheets make it harder to reuse CSS code, since the CSS rules are written within the individual web page
B. Each HTML file can only link to one external style sheet.
C. You can add external style sheets using the <style>/</style> tags.
D. Inline styles are added to an element using the style attribute and work only for that single HTML element

**Correct Answer: A & D**

6. In Javascript, what does the following comparison statement return?

```
7 === "7";
```

A. false

B. true

**Correct Answer: A**

7. In Javascript, what does the following comparison statement return?

```
7 == "7";
```

A. false

B. true

**Correct Answer: B**

8. What will be output to the console after the code runs?
```js
let myName = "Kiara";
let greeting = myName + ", Welcome to our website!"
console.log(greeting)
```

A. myName + ", Welcome to our website!"

B. myName, Welcome to our website!

C. "Kiara"", Welcome to our website!"

D. Kiara, Welcome to our website!

**Correct Answer: D**

9. What is the correct way to access guava in the fruits array?

`let fruits = ["orange", "pineapple", "guava", "jackfruit", "banana", "apple"]`

A. fruits[2]

B. fruits["guava"]

C. fruits[3]

D. fruits.guava

10. What will print to the console when the following code executes?
```js
let totals = [10,20,30,40];
for(let i=2; i < totals.length; i++){
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
20
30
```
C.
```
30
40
```
D.
```
20
40
60
80
```

11. Mentally evaluate the following code. 

```js
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
```
What will be printed to the console?

A. `"Bad Omens: The Nice and Accurate Prophecies of Agnes Nutter, Witch"`

B. `"Bad Omens:"`

C. `"Bad Omens"`

D. Reference Error

**Correct Answer: C***

12. What does are the keys in the person object?
```js
let person = {
  "name" : "E.T.",
  "homePhone" : "586-010-1982"
}
```

A. "name" and "homePhone"

B. "E.T." and "586-010-1982"

C. "name" and "homePhone", "E.T." and "586-010-1982"

**Correct Answer: A**

13. What is the difference between Git and GitHub?

A. Git is the website where users can store and manage versions of their code projects online. GitHub is the open-source system used for version control.

B. Git is a project's folder that contains all of the files for the project, as well as each file's revision history. GitHub is the open-source system used for version control.

C. Git is the open-source system used for version control. GitHub is the company that runs a website where users can store and manage versions of their code projects online.

D. Git is the open-source system used for version control.GitHub is the person who creates a repo and therefore determines if it is public or private.

**Correct Answer: C**

14. Imagine you have a local repository in a directory called git-github-assignment. You've created a new file called main.txt that has some text added to it.

What command could you run to move this file from untracked to staged?

A. git remote -v

B. git init

C. git add -A

D. git pull origin main

E. git push origin main

F. git commit -m <commit message>
  
**Correct Answer: C**
  
15. Imagine you have a local repository in a directory called git-github-assignment. You've created a new file called main.txt that is now staged.

What command could you run create a new commit with this file?
  
A. git remote -v

B. git init

C. git add -A

D. git pull origin main

E. git push origin main

F. git commit -m <commit message>
  
**Correct Answer: F**
  
16. Imagine you have a local repository in a directory called git-github-assignment. One file exists and has already been committed, called main.txt. You've created a remote repository and connected it with your local repository.

What command would you run to move your commits from your local repository to the remote repository?
  
A. git remote -v

B. git init

C. git add -A

D. git pull origin main

E. git push origin main

F. git commit -m <commit message>
  
**Correct Answer: E**
  

