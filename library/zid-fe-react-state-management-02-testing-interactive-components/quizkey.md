## React state management: Testing interactive components

1. Select all of the following statements that are true.

    **Answers:** A and B.

    A. An integration test checks whether or not individual modules of a software work properly when combined together.

    B. A unit test checks the smallest piece of logically isolated code in a program.

2. Is the following statement true or false? The React Testing Library encourages developers to write unit tests over integration tests for their React components because unit tests can test the application from the user's perspective.

    **Answer:** A. True

3. Select all statements about *mock testing* that are true.

    **Answers:** A and D.

    A. Mock testing means creating a fake version of an external or internal library that can substitute for the real one so that your tests can focus on the code being tested and not on the behavior of external systems.

    D. An example of mock testing is using a mock service in a test file to respond to the API calls made from a React component's `useEffect` hook.

4. Select the statement about test spies that is true.

    **Answer:** C. Test spies are mock functions that let you spy on the behavior of a function, rather than only testing the output of the function.

5. Select all statements that are true about the `DOM-testing-library` API.

    **Answers:** A, B, C, and D.

    A. In a test file, the `fireEvent.change()` method fires a change event on the DOM being tested.

    B. In a test file, the `fireEvent.click()` method fires a click event on the DOM being tested.

    C. In a test file, the `fireEvent.submit()` method fires a submit event on the DOM being tested.

    D. In a test file, the `screen.getByRole()` method queries for a DOM  element with a given role.

6. Select all statements that are true about the Jest library.

    **Answers:** C and D.

    C. `jest.fn()` creates a mock function which intercepts calls to the original function in a test file

    D. `jest.spyOn()` spies on an object and creates mock functions that intercept calls to the methods within the object

7. You want to test this scenario in your React application: When a user clicks on button `One` on the screen, the heading on the page should update to include the text `"Last Pressed: One"`. Which of the following tests is correctly set up to test this scenario?

    **Answer:** D.

    ```js
    test("text after clicking button One", () => {
        fireEvent.click(screen.getByRole("button", { name: /One/i }));
        expect(
          screen.getByRole("heading", { name: /Last Pressed: One/i })
        ).toBeInTheDocument();
      });
    ```

8. You are working on an existing React codebase and encounter the following test:

    ```js
    test("has correct fields", () => {
        expect(screen.queryAllByRole("textbox")).toHaveLength(2);
        expect(screen.queryAllByRole("checkbox")).toHaveLength(1);
        expect(screen.queryAllByRole("combobox")).toHaveLength(1);
      });
    ```
    True or false? The test asserts that the page should display two elements with ARIA roles `textbox`, a single element with ARIA role `checkbox`, and a single element with an ARIA role `combobox`.

    **Answer:** A. True

9. You want to test this scenario in your React application: When a user clicks on a `Get weather` button (which is inside a component called `Weather`), the page should fetch the weather information and display the information in the heading on the page with the message that starts with "The latest weather is". The `Get weather` button should then be disabled. Which of the following tests is correctly set up to test this scenario?

    **Answer:** C.

    ```js
    test('loads and displays weather', async () => {
      render(<Weather url="/weather-info" />)

      fireEvent.click(screen.getByRole(button, { name: /get weather/i }));

      await waitFor(() => screen.getByRole('heading'))

      expect(screen.getByRole('heading')).toHaveTextContent(/The latest weather is/i)
      expect(screen.getByRole('button')).toBeDisabled()
    })
    ```

10. You are working on an existing React codebase and encounter the following code in a test file:

    ```js
    const setState = jest.fn();
    const useStateMock = (initialState) => [initialState, setState];
    jest.spyOn(React, "useState").mockImplementation(useStateMock);
    ```

    What is the correct interpretation of this code?

    **Answer:** B. Spy on the `React` library, and replace the  `useState()` hook with a Jest mock so that the test file can observe its behavior during the test run.

11. Is the following statement true or false? If you're using Create React App in a project, you don't have to manually install React Testing Library because a Create React App project comes preinstalled with this library when you run `npm start`.

    **Answer:** A. True
