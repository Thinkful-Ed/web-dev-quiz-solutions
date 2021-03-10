**Node & Express: Application-level Middleware**

1. Multiple Choice Question

app.js
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

**Answer: A** `First!`

2. Multiple Choice Question

app.js
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

**Answer: B** `Second!`

3. Multiple Choice Question

app.js
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

Assume a request is made to the above server. What will be **logged** to the terminal window?

**Answer: A** `First!`

4. Multiple Choice Question

app.js
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

Assume a request is made to the above server. What will be **logged** to the terminal window?

**Answer: C** `First!` and `Second!`

5. Which of the following is a valid way to use the morgan package in your `app.js` file?

**Answer: B** `app.use(morgan("dev"));`
**Answer: C** `app.use(morgan("tiny"));`
**Answer: D** `app.use(require("morgan")("dev"));`
