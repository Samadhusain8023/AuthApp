# Authentication and Authorization Backend

This project is a backend authentication and authorization system built using Node.js, Express.js, MongoDB, JSON Web Token (JWT), and middleware. It provides user signup, login, role-based access control (RBAC), and protected routes using JWT tokens and cookies.

## Brief Explanation
This project is a **backend authentication and authorization system** designed to manage user access securely. It utilizes **JWT-based authentication** and **middleware** to protect routes based on user roles such as **Admin, Student, and Visitor**.

### Key Features:
1. **User Authentication**
   - **Signup**: Users can register with their name, email, password, and role.
   - **Login**: Authenticated users receive a **JWT token** stored in **HTTP-only cookies** for added security.
   - **Password Hashing**: Uses **bcrypt** to securely hash passwords before storing them in MongoDB.

2. **Role-Based Access Control (RBAC)**
   - Provides protected routes that allow access based on the user's role (Admin, Student, Visitor).
   - Middleware ensures only authorized users can access specific endpoints.

3. **JWT Token-Based Security**
   - Secure authentication using **jsonwebtoken (JWT)** to verify user identity.
   - Middleware extracts and validates the token from cookies or headers before granting access.

4. **Secure Cookie Storage**
   - Uses **cookie-parser** to store authentication tokens in HTTP-only cookies, preventing XSS attacks.

5. **MongoDB as Database**
   - Stores user credentials and roles securely using **Mongoose ODM**.

## Technologies Used

- **Node.js** - JavaScript runtime
- **Express.js** - Web framework for Node.js
- **MongoDB** - NoSQL database
- **Mongoose** - ODM for MongoDB
- **bcrypt** - Password hashing
- **jsonwebtoken (JWT)** - Token-based authentication
- **cookie-parser** - Parsing cookies in requests
- **dotenv** - Manage environment variables

