# Tours Api

### [Click to see API Live Demo](https://api-tours.up.railway.app/)



<hr />


### A ficitional Tour booking website made with

> -   NodeJS and ExpressJS
> -   MongoDB and Mongoose


### API BASE URL
- `/api/v1`

### API Resources URL
- `/tours`
- `/users`




### Features of the Web App

> -   Built the REST (REpresentational State Transfer) API with Node, Express and Mongoose
> -   Functionality of User Signup, login, reset account password using email is implemented
> -   Admin can delete, create and get all users, delete, create and get all tours, update and delete reviews

### Some important modules used for Security purpose

```javascript
const rateLimit = require('express-rate-limit');
const helmet = require('helmet');
const mongoSanitize = require('express-mongo-sanitize');
const xss = require('xss-clean');
const hpp = require('hpp');
const crypto = require('crypto');
const jwt = require('jsonwebtoken');
const bcrypt = require('bcryptjs');
```

> -   Rate Limit is the module used for limiting the no. of requests made by a client
> -   Helmet helps us secure our Express.js apps by securing various HTTP headers.
> -   Mongo Sanitize sanitizes mongodb queries against NOSQL query injections.
> -   XSS modules help us to prevent cross site scripting attacks.
> -   HPP module helps us to prevent attacks against HTTP parameter pollution..
> -   Crypto module used for generating hash token for reset password functionality of the user.
> -   JWT is used for stateless authentication mechanisms for users and providers.
> -   Bcrypt to hash user password and then store them in the database instead of plain password for security purposes.