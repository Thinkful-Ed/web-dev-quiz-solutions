## Redux: Core Redux concepts

1. What is Redux?

A. A pattern that enforces two-way data binding between models and views
B. A library for organizing and managing application state
C. A library for rendering UI components efficiently
D. A pattern that enforces one-way data flow in an application

**Answer: B. Redux is a library that implements the Flux pattern.**

2. In Redux, what is an action?

A. A JavaScript object containing `type` and `payload` properties.
B. A container that centralizes and manages your application's state.
C. A function that accepts the current state and an action as arguments and returns the new state.
D. The data shared across components in a Redux application

**Answer: A**

3. In Redux, what is a reducer?

A. A container that centralizes and manages your application's state.
B. A JavaScript object containing `type` and `payload` properties.
C. A function that accepts the current state and an action as arguments and returns the new state.
D. The data shared across components in a Redux application

**Answer: C**

4. In Redux, what is the difference between state and a Redux store?

A. State is a JavaScript object containing `type` and `payload` properties, whereas the Redux store is a function that accepts the current state and an action as arguments and returns the new state.
B. State is the current data used in the application, whereas the Redux store is a function that accepts the current state and an action as arguments and returns the new state.
C. State is the current data used in the application, whereas the Redux store is a container that centralizes and manages your application's state.  
D. State is a JavaScript object containing `type` and `payload` properties, whereas the Redux store is the user interface that is shown to users

**Answer: C**

5. Given the following reducer, define an `action` object that updates the state to `["A", "B", "C"]`.

```js
const reducer = (state = [], action) => {
  switch (action.type) {
    case 'addLetter':
      return [...state, action.payload];
    default:
      return state;
  }
};

// updatedState should be ['A', 'B', 'C']
const updatedState = reducer(['A', 'B'], action);
```

A.

```js
const action = {
  type: 'addLetter',
  payload: 'C',
};
```

B.

```js
const action = {
  payload: 'addLetter',
  type: 'C',
};
```

C.

```js
const action = {
  type: 'letters/addLetter',
  payload: 'C',
};
```

D.

```js
const action = {
  type: 'addLetter',
  letter: 'C',
};
```

**Answer: A**

6. In Redux, which property must an action object have?

A. `payload`
B. `dispatch`
C. `state`
D. None of the above

**Answer: D. Only the `type` property is required.**

7. Which of the following correctly describes the one-way data flow model in Redux?

A. Store -> Actions -> View -> Store
B. Store -> View -> Store -> Actions
C. Store -> View -> Actions -> Store
D. View -> Actions -> View -> Store

**Answer: C.**
