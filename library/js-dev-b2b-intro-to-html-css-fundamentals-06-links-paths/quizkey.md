**Introduction to HTML & CSS: Links & paths**

1. Which of the following options contains the correct syntax for creating an anchor element?

A. `<a to="https://www.thinkful.com" text="Thinkful" />`
B. `<a href="https://www.thinkful.com" text="Thinkful" />`
C. `<a to="https://www.thinkful.com">Thinkful</a>`
D. `<a href="https://www.thinkful.com">Thinkful</a>`

**Answer: D**

2. What is the purpose of the attribute `target="_blank"` in an anchor element?

```html   
<a href="https://www.thinkful.com" target="_blank">Link</a>
```
A. It opens the Thinkful website in a new browser window.
B. It opens the Thinkful website in a new browser tab.
C. It opens the Thinkful website and takes the user to the element with id of `"_blank"`.
D. It serves no purpose, since its value is set to `_blank`.

**Answer: B**

3. You have a folder containing some HTML, CSS, JavaScript, and image files and you have to link them together so that your web page would display properly.

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

Choose the `index.html` that is properly linked to all images, scripts, and stylesheets in the folder.

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

**Answer: B**

