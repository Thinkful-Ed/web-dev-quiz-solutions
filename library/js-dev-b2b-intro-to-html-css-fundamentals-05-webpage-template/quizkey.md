## Introduction to HTML and CSS: Web page template

1. Which of the following statements are _true_ about web page templates? You may select more than one option.

    A. `DOCTYPE` is a required first line of code that declares a document as an HTML5 web page.

    B. The `<head>` part of a HTML document holds meta information about the web page, such as the title and links to external stylesheets.

    C. `<meta name="viewport" content="width=device-width" />` is a meta tag that ensures that a web page displays properly across both desktop and mobile devices by setting the width of the web page to follow the screen width of the device the user is viewing.

    D. The `<link>` element is used to connect and reference resources on the internet.

    **Answers:** A, B, C, and D

2. Which of the following HTML element would you use to pull in JavaScript code into your HTML code? 

    A. `<script>`

    B. `<link>`

    C. `<title>`

    D. `<body>`

    **Answer:** A

3. Which part of the code below styles and formats common HTML elements so that they display consistently across web browsers?

    ```html
    <head>
      <meta charset="utf-8" />
      <meta name="viewport" content="width=device-width" />
      <title>Template: Starting Point</title>
      <link
        href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css"
        rel="stylesheet"
        type="text/css"
      />
      <link href="style.css" rel="stylesheet" type="text/css" />
    </head>

    ```

    A. `<meta charset="utf-8" />`

    B. `<meta name="viewport" content="width=device-width" />`

    C. 
      ```html
      <link
          href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css"
          rel="stylesheet"
          type="text/css"
        />
      ```

    D. `<link href="style.css" rel="stylesheet" type="text/css" />`

    **Answer:** C

4. What is a potential issue with the following code, if any?

    ```html
    <body>
      <script src="script.js"></script>
      <h1>Introduction to HTML and CSS</h1>
      <section>
        <h2>HTML Basics</h2>
        <p>HTML stands for Hypertext Markup Language.</p>
      </section>
      <section>
        <h2>CSS Basics</h2>
        <p>CSS stands for Cascading Style Sheet.</p>
      </section>
    </body>
    ```

    A. The web page may load slowly since the JavaScript code will load last.

    B. The `<section>` elements are not being used in a semantic way.

    C. The web page may load slowly since the JavaScript code needs to be loaded first before the rest of the HTML elements can be displayed on the page. 

    D. There are no potential issues with the code.

    **Answer:** C

5. Select all files or folders below that are poorly named. 

    A. `index.html`

    B. `webpage template.html`, 

    C. `about.html`

    D. `css-basics.html`

    E. `INDEX.html` 

    F. `454546asdf.html`

    G. `css_basics.html`

    H. `best-kitty-lessons.html`

    **Answers:** B, E, F, and G
