## Overview

Congratulations! You have made it this far in your learning journey, and you should be proud of your hard work and dedication. Now, it's time to put your knowledge to test with an assessment.

The assessment is designed to help you evaluate your understanding of the material covered in this module, and to identify areas where you may need to focus your studies. It consists of a series of questions that will challenge your knowledge and critical thinking skills.

Remember, assessments are an important tool for gauging your progress and ensuring that you are on track to achieving your learning goals. So, take your time, read each question carefully, and do your best.

Good luck, and let's get started!

## Learning Objective

By the end of this lesson, you will answer a set of questions that test your understanding of HTML and CSS concepts.

## Introduction to HTML and CSS: Assessment

1. Which of the following is **not** a reason for adding an `alt` attribute to an image tag?

   A. `alt` text can help the user know what image should appear on the screen if the image link is broken for some reason

   B. `alt` text can help an image load faster in a web page.

   C. `alt` text can help visual web readers to describe images to users who are blind or visually impaired.

   D. `alt` text can help search engines better interpret and therefore rank the image.

   **Answer:** B

   **Distractor Rationale: An `alt` text does not have an impact on the performance of the web page.**

2. Which of the following statements are _false_ about CSS?

   A. A CSS declaration consists of the property and value applied to the selector.

   B. Hex color codes are the only way to apply color styles to HTML elements in CSS.

   C. A CSS property describes the general category or type of stylistic change that you'd like to make.

   D. A CSS selector identifies the HTML element that should be affected by the CSS declaration.

   **Answer:** B.

   **Distractor Rationale: `white`, `#FFFFFF`, and `rgb(255,255,255)` are all valid values for the `color` property in CSS**

3. Which of the following tags would you add to a HTML file to link it to a style sheet called `style.css`?

   A. `<style href="style.css" rel="stylesheet" type="text/css" />`

   B. `<div to="style.css" rel="stylesheet" type="text/css" />`

   C. `<link href="style.css" rel="stylesheet" type="text/css" />`

   D. `<style to="style.css" rel="stylesheet" type="text/css" />`

   **Answer:** C. `<link href="style.css" rel="stylesheet" type="text/css" />`

   **Distractor Rationale: Pay special attention to the HTML tag and attributes. Keep in mind you'd need to use the correct HTML tag and attributes here.**

4. You'd like to set a font size of `16px` for all `p` elements on your web page. Which of the following syntax is correct?

   A. `p [ font-size: 16px; ]`

   B. `p { font-size: 16px; }`

   C. `p [ fontSize: 16px; ]`

   D. `p { fontSize: 16px; }`

   **Answer:** B. `p { font-size: 16px; }`

   **Distractor Rationale: CSS declarations use curly brackets and dashes (`-`) to separate words in a property name.**

5. Which of the following statements are false?

   A. You can use a `<h1>` heading more than once in a web page without getting an error.

   B. The higher the number in a heading tag, the more important that heading is. For example, `<h6>` is more important than `</h1>`.

   C. HTML headings differ in their visual style only.

   D. When creating heading elements, closing tags (e.g., `</h1>`) are optional since they make the code less readable.

   **Answer:** B., C., and D.

   **Distractor Rationale: While it is a best practice to use an `<h1>` tag only once per web page, HTML won't warn you with any visible errors if you use a <h1> tag more than once.**

6. Which of the following statement(s) are _true_ about the following CSS declaration?

   ```css
   p {
     font-family: "Gill Sans", sans-serif;
   }
   ```

   A. If "Gill Sans" is not available, then the browser will try to load a `sans-serif` font style that is available in the system.

   B. You can add more fonts in the font stack.

   C. `serif` is another reliable font fallback that can be used at the end of the font stack.

   D. All of the above.

   **Answers:** D.

   **Distractor Rationale: The code will try each font in a font stack until it finds one that works properly, and you can specify as many fonts as you want. It's generally a good idea to specify a broader type of font style, like `serif` or `sans-serif` as the final choice in the font stack.**

7. True or false? Because the `h2` element does not exist in the `index.html` page, the `h2` tag selector would apply the `color` style to the `h1` tag instead, since `h1` and `h2` are both heading tags. Therefore, `Why I love Coding` would appear in blue.

   `style.css`:

   ```css
   h2 {
     color: blue;
   }
   ```

   `index.html`:

   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <meta charset="utf-8" />
       <link href="style.css" rel="stylesheet" type="text/css" />
     </head>

     <body>
       <h1>Why I love Coding</h1>
       <p>I am awecome at coding. I can do this.</p>

       <script src="script.js"></script>
     </body>
   </html>
   ```

   A. True

   B. False

   **Answer:** B. False

   **Distractor Rationale: Tag selectors can only style the elements they're targeting, regardless of the similarity in the elements**

8. True or false? The following HTML code would result in an error.

   ```html
   <main>
     <h7>Welcome to Thinkful</h7>
     <p>This is a simple paragraph created within HTML.</p>
     <div></div>
   </main>
   ```

   A. True

   B. False

   **Answer:** B. False

   **Distractor Rationale: However, HTML won't warn you with any visible errors if you use a heading tag above <h6>, so it's up to you to keep an eye out.**

9. How many different paragraph sizes are possible in HTML? In other words, `<p1>` through what number?

A. Unlike heading elements, paragraph elements don't have sizes.

B. `<p6>`

C. `<p7>`

D. `<p8>`

**Answer:** A.

**Distractor Rationale: Do paragraph elements have sizes associated with them?**

10. You'd like to display an image on a web page and set its width to `600px`. Which of the following options are correct?

A. `<img src="images/coder.jpg" width="600"></img>`

B. `<img src="images/coder.jpg" width="600"></img>`

C. `<img src="images/coder.jpg" width="600" />`

D. `<img width="600" src="images/coder.jpg" />`

E. `<img width="600" source="images/coder.jpg" />`

F. `<img src="images/coder.jpg" alt="600" />`

**Answers:** C and D.

**Distractor Rationale: Keep in mind `img` tags are self-closing, and the order of the attributes (`src` and `width`) doesn't matter.**

11. You're creating a web page that renders a few paragraphs:

Heading: `Coffee or Tea?`
Subheading: `What do you prefer?`
Content: `The world is made up of two types of people: Coffee drinkers and tea drinkers.`

Which of the following approaches is most preferable, and why?

Approach 1:

```html
<main>
  <p>Coffee or Tea?</p>
  <p>What do you prefer?</p>
  <p>
    The world is made up of two types of people: Coffee drinkers and tea
    drinkers.
  </p>
</main>
```

Approach 2:

```html
<main>
  <h1>Coffee or Tea?</h1>
  <h2>What do you prefer?</h2>
  <p>
    The world is made up of two types of people: Coffee drinkers and tea
    drinkers.
  </p>
</main>
```

Approach 3:

```html
<main>
  <p>
    Coffee or Tea? What do you prefer? The world is made up of two types of
    people: Coffee drinkers and tea drinkers.
  </p>
</main>
```

A. Approach 1 is preferred because the use of `<p>`/`</p>` tags separates each paragraph from the one above it and the one below it. If all the tags are removed, the blocks of text will simply lump together and no longer be separated into discrete paragraphs.

B. Approach 2 is preferred because it uses the appropriate HTML elements to break up, organize, and highlight content in the web page.

C. Approach 3 is preferred because it uses only one set of `<p>` tags to display the paragraphs, thereby reducing code repetition. Since it uses fewer unnecessary HTML elements, the code is cleaner.

D. None of the above.

**Answer:** B. Approach 2 is preferred.

**Distractor Rationale: Which approach best organizes the content using the appropriate HTML elements?**

12. Which HTML tag is used to define a hyperlink?

A. <img>
B. <a>
C. <div>
D. <p>


**Answer:** B. 

**Distractor Rationale: A) `<img>` tag is used to display images on a web page. `<div>` tag is used to group and style HTML elements. `<p>` tag is used to define paragraphs of text.


