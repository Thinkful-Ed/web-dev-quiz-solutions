**React Router: Using Router, Switch, and Route**

1. True/False. An integration test checks whether or not individual modules of a software, such as individual components of a React application, work properly when combined together.

A. True
B. False

**Answer: A**

2. True/False. The React Testing Library encourages developers to write integration tests for their React components because integration tests can test the application from the user's perspective and thereby give the developer confidence that the app will work for real users.

A. True
B. False

**Answer: A**

3. The following statements describe the general steps involved in setting up a `React Testing Library` test. Select the option that places these steps in the correct order:

A. Simulate the user action on the selected DOM node
B. Render the React component into the DOM
C. Asserting that the observed outcome matches the expected outcome of interacting with the component
D. Query or select the DOM node

A. A, B, C, D
B. D, B, C, A
C. C, A, D, B
D. B, D, A, C

**Answer: D**

4. What does the `render()` method in the code below do?

```js
import { render } from '@testing-library/react';
import Greeting from '../greeting';

test('loads and displays a greeting', async () => {
  render(<Greeting />);
  // code omitted for brevity
});
```

A. It selects the `<Greeting />` component present in the DOM in the test environment
B. It simulates a click action on the `<Greeting />` component
C. It renders the `<Greeting />` component into the DOM in the test environment
D. It does nothing

5. True/False. In a test file, the `fireEvent.click()` method from the `React Testing Library` fires a change event on an input field in the form.

A. True
B. False

**Answer: B**

6. You want to test this scenario in your React application: When a user clicks on button `One` on the screen, the heading on the page should update to include the text `"Last Pressed: One"`. Which of the following tests is correctly set up to test this scenario?

A.

```js
test('text after clicking button One', () => {
  fireEvent.submit(screen.getByRole('button', { name: /One/i }));
  expect(
    screen.getByRole('heading', { name: /Last Pressed: One/i })
  ).toBeInTheDocument();
});
```

B.

```js
test('text after clicking button One', () => {
  expect(
    screen.getByRole('heading', { name: /Last Pressed: One/i })
  ).toBeInTheDocument();
  fireEvent.submit(screen.getByRole('button', { name: /One/i }));
});
```

C.

```js
test('text after clicking button One', () => {
  expect(
    screen.getByRole('heading', { name: /Last Pressed: One/i })
  ).toBeInTheDocument();
  fireEvent.click(screen.getByRole('button', { name: /One/i }));
});
```

D.

```js
test('text after clicking button One', () => {
  fireEvent.click(screen.getByRole('button', { name: /One/i }));
  expect(
    screen.getByRole('heading', { name: /Last Pressed: One/i })
  ).toBeInTheDocument();
});
```

**Answer: D**

7. You want to test this scenario in your React application: When a user clicks on a `Get weather` button (which is inside a component called `Weather`), the page should fetch the weather information and display the information in the heading on the page with the message that starts with "The latest weather is". The `Get weather` button should then be disabled. Which of the following tests is correctly set up to test this scenario?

A.

```js
test('loads and displays weather', async () => {
  render(<Weather url="/weather-info" />);

  fireEvent.click(screen.getByRole('button', { name: /get weather/i }));

  await waitFor(() => screen.getByRole('heading'));

  expect(screen.getByRole('heading')).toHaveTextContent(
    /The latest weather is/i
  );
});
```

B.

```js
test('loads and displays weather', async () => {
  render(<Weather url="/weather-info" />);

  await waitFor(() => screen.getByRole('heading'));

  fireEvent.submit(screen.getByRole('button', { name: /get weather/i }));

  expect(screen.getByRole('heading')).toHaveTextContent(
    /The latest weather is/i
  );
});
```

C.

```js
test('loads and displays weather', async () => {
  render(<Weather url="/weather-info" />);

  fireEvent.click(screen.getByRole(button, { name: /get weather/i }));

  await waitFor(() => screen.getByRole('heading'));

  expect(screen.getByRole('heading')).toHaveTextContent(
    /The latest weather is/i
  );
  expect(screen.getByRole('button')).toBeDisabled();
});
```

D.

```js
test('loads and displays weather', async () => {
  render(<Weather url="/weather-info" />);

  fireEvent.click(screen.getByRole('button', { name: /submit/i }));

  await waitFor(() => screen.getByRole('heading'));

  expect(screen.getByRole('heading')).toHaveTextContent(
    /The latest weather is/i
  );
});
```

**Answer: C**

8. Is the following statement true or false? If you're using Create React App in a project, you don't have to manually install React Testing Library because a Create React App project comes preinstalled with this library when you run `npm start`.

A. True
B. False

**Answer: A**
