## Backend deployment: Deploying a monorepo

1. True/False. A monorepo is a repository that contains both the client and the backend projects.

A. True
B. False

**Answer: A**

1. You're deploying the backend of a monorepo with the following folder structure and need to specify a root directory in the deployment configuration for deploying **only** the backend. Which value would you specify?

.
├── README.md
├── backend
│ ├── README.md
│ ├── generator.js
│ ├── node_modules
│ ├── package-lock.json
│ ├── package.json
│ ├── routes.js
│ └── server.js
├── frontend
│ ├── README.md
│ ├── build
│ ├── node_modules
│ ├── package-lock.json
│ ├── package.json
│ ├── public
│ └── src
├── package-lock.json
└── package.json

A. `backend`
B. `frontend`
C. `client`
D. `public`

**Answer: A**

1. You're deploying the frontend of a monorepo with the following folder structure and need to specify a root directory in the deployment configuration for deploying **only** the client code. Which value would you specify?

.
├── README.md
├── backend
│ ├── README.md
│ ├── generator.js
│ ├── node_modules
│ ├── package-lock.json
│ ├── package.json
│ ├── routes.js
│ └── server.js
├── frontend
│ ├── README.md
│ ├── build
│ ├── node_modules
│ ├── package-lock.json
│ ├── package.json
│ ├── public
│ └── src
├── package-lock.json
└── package.json

A. `backend`
B. `frontend`
C. `client`
D. `public`

**Answer: B**
