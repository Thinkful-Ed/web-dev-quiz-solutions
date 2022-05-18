## Introduction to HTML and CSS: CSS basics

1. Which of the following statements are _true_ about CSS? 

	A. A CSS declaration consists of the property and value applied to the selector.

	B. A CSS property describes the general category or type of stylistic change that you'd like to make.

	C. A CSS selector identifies the HTML element that should be affected by the CSS declaration.

	D. All of the above

	**Answer:** D. All of the above

2.  Which of the following tags would you add to a HTML file to link it to a style sheet called `style.css`?

	A. `<link href="style.css" rel="stylesheet" type="text/css" />`

	B. `<link to="style.css" rel="stylesheet" type="text/css" />`

	C. `<style href="style.css" rel="stylesheet" type="text/css" />`

	D. `<style to="style.css" rel="stylesheet" type="text/css" />`

	**Answer:** A. `<link href="style.css" rel="stylesheet" type="text/css" />`

3. You'd like to set a background color of `red` for all `div` elements on your web page. Which of the following syntax is correct?

	A. `div [ background-color: red; ]`

	B. `div { background-color: red; }`

	C. `div [ backgroundColor: red; ]`

	D. `div { backgroundColor: red; }`

	**Answer:** B. `div { background-color: red; }`

4. Which of the following statement(s) are _true_ about the following CSS declaration?

	```css
	p {
	  font-family: "Fancy", Futura, sans-serif;
	}
	```

	A. If "Fancy" is not available, then the browser will try to load Futura instead.

	B. `sans-serif` is a broader font style that serves as a reliable fallback.

	C. If "Fancy" and Futura are not available, then the browser will try to load any available `sans-serif` font in the system.

	D. You're limited to listing only three fonts in the font stack.

	**Answers:** A, B, and C

5. True or false? The following code setup would cause an error because the CSS file is targeting an element that that doesn't exist in the HTML.

	`index.html`:
	```html
	<!DOCTYPE html>
	<html>

	<head>
		<meta charset="utf-8">
		<link href="style.css" rel="stylesheet" type="text/css" />
	</head>

	<body>

		<h1>Header</h1>
		<p>This is a one sentence paragraph.</p>

		<script src="script.js">
		</script>
	</body>

	</html>
	```

	`style.css`:
	```css
	h2 {
	  text-align: center;
	}
	```
	
	A. True
	
	B. False

	**Answer:** B. False
