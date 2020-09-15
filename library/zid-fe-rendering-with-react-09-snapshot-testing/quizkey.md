**Rendering in React: Thinking in React**

1. True or False: Every time you run a snapshot test, a new snapshot is created and saved.
**Answer: B**  False

2. Which of the following is correct for creating a snapshot of the `App` component?

Assume you have the following import statements.

```js
import React from "react";
import { create } from "react-test-renderer";
import App from "./App";
```

**Answer: B**
`expect(create(<App />).toJSON()).toMatchSnapshot()`
