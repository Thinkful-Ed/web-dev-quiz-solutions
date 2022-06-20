## Redux: Rules of reducers

1. Which of these are rules of reducers? Select all that apply.

A. Reducers must only perform asychronous logic or "side effects"
B. Reducers must only use `switch` statements, instead of `if-else` statements, to evaluate action types
C. Reducers must only use the current state and action arguments to determine the new state value
D. Reducers must make a copy of, instead of directly modify, the existing state

**Answers:C & D**

2. In Redux, which of the following are valid examples of "side effects" that should be avoided inside a reducer function? Select all that apply.

A. Making a HTTP call to a RESTful API
B. Calling `setInterval()`
C. Calling `const name = "John";`
D. Calling `console.log()`

**Answers: A, B, & D**

3. Given the reducer function below, complete the `addPost` function so that it updates `state` immutably. The new post to be added can be accessed via `action.payload`.

```js
const postReducer = (state = [], action) => {
  switch (action.type) {
    case 'addPost':
      return /* fill in the blank */;
    default:
      return state;
  }
};
```

A. `[...state, action.payload]`;
B. `state.push(action.payload)`;
C. `[action.payload]`;
D. `[state, action.payload]`

**Answer: A. Use the spread operator `...` to make a copy of the state value.**

4. Given the reducer function below, complete the `setToGraduated` function so that it updates state immutably. The `setToGraduated` action should set the `isGraduated` property to `true`.

```js
const initialState = {
  isGraduated: false,
  name: 'John',
  level: 'senior',
};

const studentReducer = (state = initialState, action) => {
  switch (action.type) {
    case 'setToGraduated': {
      return /* fill in the blank */;
    }
    default:
      return state;
  }
};
```

A.

```js
{
  state,
  isGraduated: true
}
```

B.

```js
{
  state.name,
  state.level,
  isGraduated: true
}
```

C.

```js
{
  [...state],
  isGraduated: true
}
```

D.

```js
{
  ...state,
  isGraduated: true
}
```

**Answer: D**

5. True/False. The reducer function below is valid:

```js
const reducer = (action) => {
  switch (action.type) {
    case 'increment': {
      return 1;
    }
    default: {
      return 0;
    }
  }
};
```

A. True
B. False

**Answer: B. A reducer must accept two parameters: `state` and `action`**
