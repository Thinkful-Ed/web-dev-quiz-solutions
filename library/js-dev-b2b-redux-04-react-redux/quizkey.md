## Redux: `react-redux`

1. Given the state object below, how would you create a Redux selector that returns an array of posts?

```js
state = {
  posts: [
    { id: 1, title: 'First blog post', body: 'Some content' },
    { id: 2, title: 'Second blog post', body: 'Some content' },
    { id: 3, title: 'Third blog post', body: 'Some content' },
  ],
};
```

A. `export const selectPosts = state => posts`
B. `export const selectPosts = () => posts`
C. `export const selectPosts = state => state.posts`
D. `export const selectPosts = () => state.posts`

**Answer: C**

2. Complete the code below so that the components nested further down in the application can access the Redux store without having to pass the store via props.

```js
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from "react-redux";

import App from './src/app/App';
import { store } from './src/app/store.js';

ReactDOM.render(
  /* fill in the blank */
  ,
  document.getElementById('root')
);

```

A.

```js
<Provider>
  <App store={store} />
</Provider>
```

B.

```js
<store>
  <App />
</store>
```

C.

```js
<Provider>
  <App />
</Provider>
```

D.

```js
<Provider store={store}>
  <App />
</Provider>
```

**Answer: D**

3.  Which of the following statements about `useDispatch()` is true? Select only one answer.

A. It references the dispatch function in the Redux store
B. It references an action object
C. It references an action creator
D. It dispatches an action using an action creator

**Answer: A**

4. Which of the following statements about `react-redux` package are true? Select all that apply.

A. It is the only any to manage React application state
B. It is maintained by the Redux team
C. It allows only the top-level application component to dispatch actions to the Redux store
D. It allows any application component to subscribe to updates in specific "slices" of the global state

**Answer: B & D**

5. Complete the code below so that the `Posts` component re-renders based on changes in the `selectPosts` data only

```js
// Posts.js
import /* (1) fill in the blank */ 'react-redux';
import { selectPosts } from 'postsSlice.js';

export default function Posts() {
  const posts = /* (2) fill in the blank */ selectPosts;

  return <div>{posts}</div>;
}
```

A. (1) `useSelect`, (2) `useSelect`
B. (1) `useDispatch`, (2) `useDispatch`
C. (1) `useDispatcher`, (2) `useDispatcher`
D. (1) `useSelector`, (2) `useSelector`

**Answer: D**

6. Which of the following commands would you use to install the `react-redux` library?

A. `npm install react-redux`
B. `npm install redux`
C. `npm install react-redux-binding`
D. `npm install react`

**Answer: A**
