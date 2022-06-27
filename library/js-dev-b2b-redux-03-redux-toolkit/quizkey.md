## Redux: Redux Toolkit

1. Which of the following statements about Redux Toolkit is false?

A. It contains a library of reusable React components to boost developer productivity
B. It simplifies the code for setting up Redux in an application, including actions, reducers, store, action creators, and thunks
C. It is built with best practices in mind and simplifies Redux tasks such as integrating with the Redux DevTools
D. It uses the `configureStore()` method to simplify the store setup process.

**Answer: A**

2. The `options` object passed to `createSlice()` includes all of following properties EXCEPT

A. `initialState`
B. `name`
C. `actions`
D. `reducers`

**Answer: C. RTK will automatically generate the action creators for each case reducer, so there's no need to explicitly define the action creators.**

3. Given the following code, which argument would you pass to `configureStore()` to setup the Redux store for the application?

```js
import { configureStore } from '@reduxjs/toolkit';
import postsReducer from './features/posts/postsSlice';
import usersReducer from './features/users/usersSlice';

const store = configureStore();
//...
```

A.

```js
const store = configureStore({
  posts: postsReducer,
  users: usersReducer,
});
```

B.

```js
const store = configureStore(postsReducer, usersReducer);
```

C.

```js
const store = configureStore({
  reducer: {
    posts: postsReducer,
    users: usersReducer,
  },
});
```

D.

```js
const store = configureStore({
  reducer: [postsReducer, usersReducer],
});
```

**Answer: C**

4. Which of the following are properties of the object returned by `createSlice()`? Select all that apply.

A. `initialState`
B. `actions`
C. `name`
D. `reducer`

**Answer: B, C, & D**

5. Give the code below, select all statements that are true about the code snippet:

```js
const blogSlice = createSlice({
  name: "blog",
  initialState: [],
  reducers: {
    addPost: (state, action) => {
      state.push(action.payload);
    },
    removePost: (state, action) => {
      return state.filter(item => item.id !== action.payload.id)
    },
    default: (state, action) {
      return state;
    }
  },
});
```

A. The `addPost` reducer will mutate the existing `state` array because it uses `state.push()`
B. Defining the `default` case reducer in `reducers` is necessary to prevent an error in the application if the dispatched action matches none of the defined action types
C. The `reducers` property should be called `extraReducers`
D. None of the above

**Answer: D**

6. You're building an app and would like to setup Redux quickly. Which of the following package would you install that will allow you to save time and take advantage of Redux best practices?

A. `npm install react`
B. `npm install @reduxjs/toolkit`
C. `npm install redux`
D. `npm install react-redux`

**Answer: B. The `@reduxjs/toolkit` package provides the `createSlice()` and `configureStore()` methods to simplify Redux setup.**

7. True/False. The Redux Toolkit allows React components to talk to the Redux store using `createSlice()`.

A. True
B. False

**Answer: B. The Redux Toolkit was not created to solve the problem of connecting React components to the Redux store.**
