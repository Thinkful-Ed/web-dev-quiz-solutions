**React Router: Intro to frontend routing**

1. True/False. In an application that uses frontend routing, the client(browser) makes a request to the server every time the user navigates to a new page in the app.

A. True
B. False

**Answer: B. False**

2. What are the potential benefits of frontend routing? Select all that applies.

A. Routing between frontend views is generally faster than backend routing.
B. It allows visitors to share links to specific content and pages.
C. It allows visitors to bookmark pages
D. All of the above.

**Answer: D. All of the above**

3. Imagine the following React application is running in the browser. Select the statements that are true. Pick two. 

```js
import React from "react";

function Home() {
  return <p>Home</p>;
}

function About() {
  return <p>About</p>;
}

function App() {
  return (
    <div className="App">
      {window.location.pathname === "/about" ? <About /> : <Home />}
    </div>
  );
}

export default App;
```

A. Navigating to the `/contact` path takes the user to the `About` component
B. Navigating to the `/contact` path takes the user to the `Home` component
C. Navigating to the `/home` path takes the user to the `Home` component
D. Navigating to the `/about` path takes the user to the `Home` component

**Answer: B, C**

4. True/False. Routing is the process of keeping the browser URL in sync with what's being displayed on the page.

A. True
B. False

**Answer: A**
