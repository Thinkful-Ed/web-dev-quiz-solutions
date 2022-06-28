
1 - Which of the following refers to a system that confirms the identity of a user (for example, requiring login credentials like a username and password)?

A. Authorization

B. Authentication

C. JWT

D. localStorage

**Answer: B**

2 - Which of the following refers to a system that determines who has access to what (for example, having admin-only views in an app)?

A. Authorization

B. Authentication

C. JWT

D. localStorage

**Answer: A**

3 - Which of the following are compact and self-contained tokens for transmitting data between parties?

A. Authorization

B. Authentication

C. JWT

D. localStorage

**Answer: C**

4 - Which of the following options can you use to save the JWT token in the client?

A. localStorage

B. sessionStorage

C. cookies

D. all of the above

**Answer: D**

5 - In the code snippet below:

```
<Route path='/profile' element={
  <Protected>
    <Profile />
  </Protected>
}
```
What is the purpose of the <Protected> component?

A. It only allows authenticated users to access the Profile page.

B. It adds additional layers of security using high-level encryption.

C. It's a component that adds security features to the Profile page.

D. None of the above

**Answer: A**
  
6 - Which of the following allows you to add data to localStorage?

A. localStorage.setItem('token', 'pretend this is a JWT token');

B. localStorage.addItem('token', 'pretend this is a JWT token');

C. localStorage.pushItem('token', 'pretend this is a JWT token');

D. localStorage.getItem('token', 'pretend this is a JWT token');

**Answer: A**
  
7. Which of the following best describes the typical authentication flow with JWT?

A.
  ```
The server returns a JWT (signed with a key).
The client sends user credentials (username and password) to the server.
In the client, JWT is stored in localStorage.
In the client, JWT is sent on every request to the server.
  ```
B.
  ```
The client sends user credentials (username and password) to the server.
In the server, JWT is stored in localStorage.
The server returns a JWT (signed with a key).
In the client, JWT is sent on every request to the server.
```
C. 
  ```
The server sends user credentials (username and password) to the client.
The client returns a JWT (signed with a key).
In the server, JWT is stored in localStorage.
In the client, JWT is sent on every request to the server.
```
D.
  ```
The client sends user credentials (username and password) to the server.
The server returns a JWT (signed with a key).
In the client, JWT is stored in localStorage.
In the client, JWT is sent on every request to the server.
  ```
**Answer: D**
  
8 - What is the purpose of `axios.defaults.headers.common["Authorization"] = token;`?

A. This will embed the JWT token in any new request that the client sends to the server.

B. This will embed the username in any new request that the client sends to the server.

C. Gives the server the user's credentials.

D. None of the above

**Answer: A**
