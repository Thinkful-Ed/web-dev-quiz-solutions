## Node and Express: Application-level middleware

1. `app.js`

    ```js
    const express = require('express')
    const app = express()

    const first = (req, res, next) => {
      res.send('First!')
    }

    const second = (req, res, next) => {
      res.send('Second!')
    }

    app.use(first)
    app.use(second)

    module.exports = app
    ```

    Assume a request is made to the above server. What would the response be?

    **Answer:** A. `First!`

2. `app.js`

    ```js
    const express = require('express')
    const app = express()

    const first = (req, res, next) => {
      return next()
      res.send('First!')
    }

    const second = (req, res, next) => {
      res.send('Second!')
    }

    app.use(first)
    app.use(second)

    module.exports = app
    ```

    Assume a request is made to the above server. What would the response be?

    **Answer:** B. `Second!`

3. `app.js`

    ```js
    const express = require('express')
    const app = express()

    app.use((req, res, next) => {
      console.log('First!')
      res.send('Done.')
    })
    app.use((req, res, next) => {
      console.log('Second!')
      res.send('Done.')
    })

    module.exports = app
    ```

    Assume a request is made to the above server. What will be *logged* to the terminal window?

    **Answer:** A. `First!`

4. `app.js`

    ```js
    const express = require('express')
    const app = express()

    app.use((req, res, next) => {
      console.log('First!')
      next()
    })
    app.use((req, res, next) => {
      console.log('Second!')
      res.send('Done.')
    })

    module.exports = app
    ```

    Assume a request is made to the above server. What will be *logged* to the terminal window?

    **Answer:** C. `First!` and `Second!`

5. Which of the following is a valid way to use the morgan package in your `app.js` file?

    **Answers:** B, C, and D.
    
    B. `app.use(morgan("dev"));`
    
    C. `app.use(morgan("tiny"));`
    
    D. `app.use(require("morgan")("dev"));`
