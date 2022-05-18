## Deeper with CSS: Classes

1. Select all statements that are _true_ about CSS style sheets.

	A. Each HTML file can only link to one external style sheet.

	B. Internal style sheets make it harder to reuse CSS code, since the CSS rules are written within individual web pages.

	C. You can add external style sheets using the `<style>`/`</style>` tags.

	D. Inline styles are added to an element using the `style` attribute and work only for that single HTML element

	**Answers:** B and D

2. Given the following HTML and CSS files, what will be observed when the web page is loaded in the browser? 

	```html
	<!DOCTYPE html>
	<html>
	<head>
	  <style>
	    .title {
	      color: red;
	    }
	  </style>
	  <link rel="stylesheet" type="text/css" href="style.css" />
	</head>
	<body>
	  <h1 style="color: yellow;" class="title">Welcome to Thinkful</h1>
	</body>
	</html>
	```

	```css
	.title {
	  color: green;
	}
	```

	A. `Welcome To Thinkful` appears in red.

	B. `Welcome To Thinkful` appears in yellow.

	C. `Welcome To Thinkful` appears in green.

	D. The browser displays an error.

	**Answer:** B

3. You're building a web page, but the style of the paragraph isn't changing even though you're certain that a rule you wrote should be causing the style to change. What could the issues be? You may select more than one response.

	A. You forgot to add a `<script>` tag to your HTML file

	B. You forgot to link an external style sheet containing the desired CSS rules to your HTML file

	C. A higher priority rule is overriding the CSS rule you wrote for the paragraph 

	D. The CSS rule for the paragraph is overriding another rule

	**Answers:** B and C

4. True or false? `!important` tells the code that a certain CSS rule should override other rules even though it might be lower priority in the cascade.

	A. True

	B. False

	**Answer:** A

5. What is one key benefit of using classes?

	A. Classes allow you to apply a set of CSS properties to a specific HTML element only.

	B. Using class selectors is more performant and secure than using element selectors.

	C. Using class selectors requires you to apply styling with an external style sheet.

	D. Classes allow you to apply a set of CSS properties to any HTML element and reuse them throughout a web page.

	**Answer:** D

6. You would like to apply multiple classes to a `h1` element on a web page:

	```css
	.error {
	  color: red;
	}

	.large {
	  font-size: 35px;
	}
	```

	Which HTML syntax is correct?

	A. `<h1>Internal server error.</h1 class="error large">`

	B. `<h1 class="error" class="large">Internal server error.</h1>`

	C. `<h1 classes="error large">Internal server error.</h1>`

	D. `<h1 class="error large">Internal server error.</h1>`

	**Answer:** D

7. Given the following HTML and CSS files, what will happen?

	`index.html`:
	```html
	<!DOCTYPE html>
	<html>

	<head>
		<meta charset="utf-8">
		<link href="style.css" rel="stylesheet" type="text/css" />
	</head>

	<body>

		<h1 class="center">Header</h1>
		<p class="center">This is a one sentence paragraph.</p>

		<script src="script.js">
		</script>
	</body>

	</html>
	```

	`style.css`:
	```css
	h1.center {
	  text-align: center;
	}
	```

	A. Both `Header` and `This is a one sentence paragraph.` will be centered on the page.

	B. Only the `Header` will be centered on the page.

	C. Only `This is a one sentence paragraph.` will be centered on the page.

	D. Neither text would be centered since `h1.center` is *not* a valid CSS selector syntax.

	**Answer:** B

8. You would like *all* `<h2>` headings nested within `<section>` containers to have a font-size of `35px`. Which of the following CSS selector would you apply?

	A. `section > h2 { font-size: 35px }`;

	B. `section h2 { font-size: 35px }`; 

	C. `section.h2 { font-size: 35px }`;

	D. `section < h2 { font-size: 35px }`;

	**Answer:** B
