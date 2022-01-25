## React Hooks: JWT Authentication (without Redux) example

For more detail, please visit:

> [React Hooks: JWT Authentication & Authorization example](https://bezkoder.com/react-hooks-jwt-auth/)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### Set port
.env
```
PORT=8081
```

## Note:
Open `src/services/auth-header.js` and modify `return` statement for appropriate back-end (found in the tutorial).

```js
export default function authHeader() {
  const user = JSON.parse(localStorage.getItem('user'));

  if (user && user.accessToken) {
    // return { Authorization: 'Bearer ' + user.accessToken }; // for Spring Boot back-end
    return { 'x-access-token': user.accessToken };             // for Node.js Express back-end
  } else {
    return {};
  }
}
```

## Project setup

In the project directory, you can run:

```
npm install
# or
yarn install
```

or

### Compiles and hot-reloads for development

```
npm start
# or
yarn start
```

Open [http://localhost:8081](http://localhost:8081) to view it in the browser.

The page will reload if you make edits.














Build an application for trading. You need to do the user registration of the user with email verification. After the verification of the user account. Users can login and can see a number of things in the project.

Registration Form:
Name -Km Roshni
Email -r39992510@gmail.com
Password
Photo (use base 64 string method)

Login process:
Login will be done using the JWT implementation


After login, users can see trading information in the application. Think about the user accessibility and implement the features on the UI.

Implemente the trade data of stock.
Use API: https://polygon.io/docs/get_v2_ticks_stocks_trades__ticker___date__anchor
API Doc: https://polygon.io/docs

Write the Unit Testing of any one Module

What we check:
Code Optimization  -- 10 Marks
Feature Implementation -- 10 Marks
API Implementation and handling the large Data -- 20 Marks
Github Uploading and Documentation of the Project (You need to submit a instructions, How to run the project) -- 10 Marks
Marks: 50 
 
Submission Date: Mentioned In the Email
24/01/2022

