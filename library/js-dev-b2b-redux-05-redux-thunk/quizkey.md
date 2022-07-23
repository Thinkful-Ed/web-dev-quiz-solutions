## Redux: Redux Thunk

1. True/False. `redux-thunk` allows you to write action creators that return functions or objects.

A. True
B. False

**Answer: A**

2. True/Fase. In the Redux data flow, a middleware runs after an action is dispatched to the store.

A. True
B. False

**Answer: B**

3. Fill in the blank with the most appropriate response. What is a thunk? It's a special function that \_\_\_.

A. is returned by another function and contains logic that can be executed later on
B. accepts only a single argument
C. must accept a function as one of its arguments
D. returns a function that is executed immediately

**Answer: A**

4. `createAsyncThunk` creates an asynchronous action creator that dispatches synchronous actions for each of the promise lifecycle states (i.e., `pending`, `fulfilled`, and `rejected`). Select the statements that are true about the code given below. Select all that apply.

```js
import { fetchPost } from 'api';

const fetchPostById = createAsyncThunk(
  'posts/fetchPostById',
  async (postId) => {
    const post = await fetchPost(postId);
    return post;
  }
);
```

A. `posts/fetchPostById` defines the action type
B. `posts/fetchPostById` defines the configuration options
C. `async (postId) => { const post = await fetchPost(postId); return post;}` defines the asynchronous thunk function
D. `async (postId) => { const post = await fetchPost(postId); return post;}` defines the synchronous thunk function

**Answer: A & D**

5. What is the benefit of adding middleware in Redux?

A. It prevents you from accidentally writing asynchronous logic within the reducer
B. It intercepts dispatched actions and allows you to perform asynchronous operations such as API calls
C. It allows your React components to talk to the Redux store
D. It immediately passes dispatched actions to the store's reducer

**Answer: B**

6. Complete the code below to set up a Redux store using the `redux-thunk` middleware.

```js
/* (1) fill in the blank */
import productsReducer from '../features/products/productsSlice';

export default /* (2) fill in the blank */ {
  reducer: {
    products: productsReducer,
  },
};
```

A. (1) `import { createStore } from "redux";` (2) `createStore`
B. (1) `import { configureStore } from "@reduxjs/toolkit";` (2) `configureStore`
C. (1) `import { createStore } from "@reduxjs/toolkit";` (2) `createStore`
D. (1) `import { configureStore } from "redux";` (2) `configureStore`

**Answer: B**

7. True/False. When using `createAsyncThunk()`, you can make your reducers respond to `pending`/`fulfilled`/`rejected` promise lifecycle actions by adding the `reducers` property to the configuration object passed to `createSlice()`.

A. True
B. False

**Answer: B. You need to add `extraReducers`, not `reducers`.**

8. Given the code below, fill in the blanks with the appropriate actions.

```js
import { createAsyncThunk, createSlice } from "@reduxjs/toolkit";

export const loadProducts = createAsyncThunk(
  "products/loadProducts",
  async () => {
    const response = await fetch("api/products?limit=100");
    const products = await response.json();
    return products;
  }
);

export const productsSlice = createSlice({
  name: "products",
  initialState: {
    products: [],
    loading: false,
    error: false
  },
  extraReducers: {
    [/* fill in the blank (1) */]: (state, action) => {
      state.loading = true;
      state.error = false;
    },
    [/* fill in the blank (2) */]: (state, action) => {
      state.recipes = action.payload;
      state.loading = false;
      state.error = false;
    },
    [/* fill in the blank (3) */]: (state, action) => {
      state.loading = false;
      state.error = true;
    }
  }
});

export default productsSlice.reducer;
```

A. (1) `loadProducts.fulfilled`, (2) `loadProducts.rejected`, (3) `loadProducts.pending`
B. (1) `loadProducts.pending`, (2) `loadProducts.rejected`, (3) `loadProducts.fulfilled`
C. (1) `loadProducts.pending`, (2) `loadProducts.fulfilled`, (3) `loadProducts.rejected`
D. (1) `products/loadProducts.pending`, (2) `products/loadProducts.fulfilled`, (3) `products/loadProducts.rejected`

**Answer: C**
