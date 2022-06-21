1 - Which of the following code snippets would you use in the index.js file of a React 18 app?

A. 
```js
import React from "react";
import ReactDOM from "react-dom";
import "./index.css";
import App from "./App";

ReactDOM.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById("root")
);
```

B.
```js
import React from "react";
import ReactDOM from "react-dom/server";
import "./index.css";
import App from "./App";

ReactDOM.root(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById("root")
);
```

C.
```js
import React from 'react';
import ReactDOM from 'react-dom/server';
import './index.css';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

D.
```js
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

**Answer: D**

2 - Which of the following would you use to remove a mounted component in React 18?

A. unmountComponentAtNode(container);

B. unmount();

C. root.unmountComponentAtNode(container);

D. root.unmount();

**Answer: D**

3 - The createRoot() method replaces the ReactDOM.render method that is used in React 17.

A. True

B. False

**Answer: A**

4 - In React 18, transition updates are direct user interactions such as typing and clicking.

A. True

B. False

**Answer: B**

5 - Which of the following is NOT a new feature in React 18?

A. transitions

B. automatic batching

C. client and server rendering APIs

D. one-way data binding

**Answer: D**

6 - Before React 18, rendering couldn't be paused and resumed.

A. True

B. False

**Answer: A**
