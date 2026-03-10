BASIC AUTHENTICATION SYSTEM

Overview
This project demonstrates a simple Basic Authentication System that includes:
- Signup
- Login
- Logout
- Password hashing using bcrypt
- JWT (JSON Web Token) authentication for protected routes

The system ensures that user credentials are stored securely and that only authenticated users can access protected resources.


Features

1. Signup
Users can create a new account by providing:
- Email
- Password

The password is hashed using bcrypt before being stored in the database to improve security.

2. Login
Registered users can log in by entering their email and password.
The system verifies the password by comparing it with the stored bcrypt hash.

3. Logout
Users can log out of the system, which invalidates their authentication token or session.

4. Password Hashing (bcrypt)
bcrypt is used to securely hash passwords.

Advantages:
- Protects passwords from being stored in plain text
- Includes salting to prevent common attacks
- Makes password cracking computationally difficult

5. JWT Authentication
After a successful login, the system generates a JWT token.

This token is used to:
- Authenticate future requests
- Access protected routes
- Maintain user session securely


How the System Works

1. User signs up with email and password.
2. Password is hashed using bcrypt and stored securely.
3. User logs in using credentials.
4. Server verifies password and generates a JWT token.
5. Token is sent with requests to access protected routes.
6. Server validates the token before granting access.


Technologies Used

- HTML / CSS
- JavaScript
- bcrypt (Password Hashing)
- JWT (Authentication)
- Node.js / Backend Authentication Logic


Project Purpose

The purpose of this project is to demonstrate how modern web applications handle:
- Secure user authentication
- Password protection
- Token-based authorization

This system is commonly used in web applications, APIs, and modern full-stack projects.
