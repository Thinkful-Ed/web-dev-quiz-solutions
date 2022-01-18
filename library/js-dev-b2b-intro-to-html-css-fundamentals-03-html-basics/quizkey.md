**Introduction to HTML & CSS: HTML Basics**

1. True/False. The following HTML code is correctly written:

```html
<main>
  <h1>Welcome to Thinkful<h1>
  <p>This is a simple paragraph created within HTML.<p>
</main>
```

A. TRUE
B. FALSE 

**Answer: B (because the closing tags for heading and paragraph elements should be `</h1>` and `</p>`, respectively)**

2. You're creating a web page that renders a few paragraphs. Which of the following approaches is more preferable than the other and why? 

`Approach 1`:
```html
<main>
  <p>My first paragraph</p>
  <p>My second paragraph</p>
  <p>My third paragraph</p>
</main>
```

`Approach 2`:
```html
<main>
  My first paragraph
  My second paragraph
  My third paragraph
</main>
```

`Approach 3`:
```html
<main>
  <p>
    My first paragraph
    My second paragraph
    My third paragraph
  </p>
</main>
```
 
A. Approach 1 is preferred because the use of `<p>`/`</p>` tags separates each paragraph from the one above it and the one below it. If all the tags are removed, the blocks of text will simply lump together and no longer be separated into discrete paragraphs.
B. Approach 2 is preferred because it uses fewer unnecessary HTML elements. The code is cleaner without the use of `<p>` elements to display the paragraphs. 
C. Approach 3 is preferred because it uses only one set of `<p>` tags to display the paragraphs, thereby reducing code repetition.
D. Neither.

**Answer: A**

3. How many different heading sizes are possible in HTML (in other words, `<h1>` through what number)?

A. `<h5>`
B. `<h6>`
C. `<h7>`
D. `<h8>`

**Answer: B**

4. Which of the following statement(s) is/are false?

A. The higher the number in a heading tag, the more important that heading is (e.g., `<h6>` is more important than `</h1>`)  
B. If you try to use a `<h1>` heading more than once in a web page, you will get an error.
C. HTML headings differ in their visual style only.
D. All of the above.

**Answer: D**

5. You'd like to display an image on a web page and set its width to `600px`. Which of the following options is/are correct? 

A.
```html
<img src="images/mountain-hiker.jpg" width="600"></img>
```

B.
```html
<img src="images/mountain-hiker.jpg" width="600"></img>
```

C. 
```html
<img src="images/mountain-hiker.jpg" width="600" />
```

D. 
```html
<img width="600" src="images/mountain-hiker.jpg" />
```

E.
```html
<img width="600" source="images/mountain-hiker.jpg" />
```

F.
```html
<img src="images/mountain-hiker.jpg" alt="600" />
```
**Answer: C, D (the order of the attributes does not matter)**

6. Why is it important to add an `alt` attribute to an image tag?

A. Visual web readers can use `alt` text to describe images to users who are blind or visually impaired.
B. `alt` text can help search engines better interpret and therefore rank the image.
C. `alt` text can help the user know what image should appear on the screen if the image link is broken for some reason
D. All of the above

**Answer: D**
