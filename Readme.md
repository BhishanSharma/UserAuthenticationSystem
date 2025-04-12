# User Authentication System

A web-based user authentication system that supports **Google OAuth** for login and **JWT** for session management. This system allows users to log in via Google, register, and handle authentication states securely.

## Features

- **Google OAuth Login**: Secure authentication using Google credentials.
- **JWT Authentication**: Manage user sessions with JSON Web Tokens (JWT).
- **User Registration**: Allows users to register using their email and password.
- **Logout**: Secure logout functionality.

## Requirements

- Node.js
- MongoDB
- Google Developer Console credentials

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/BhishanSharma/UserAuthenticationSystem.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set environment variables:
   ```env
   GOOGLE_CLIENT_ID=<Your Google Client ID>
   GOOGLE_CLIENT_SECRET=<Your Google Client Secret>
   GOOGLE_CALLBACK_URL=<Your Google Callback URL>
   ACCESS_TOKEN_SECRET=<Your Access Token Secret>
   REFRESH_TOKEN_SECRET=<Your Refresh Token Secret>
   ```
4. Run the server:
   ```bash
   npm start
   ```

## Routes

- **POST /register**: Register a new user.
- **POST /login**: Login with username/email and password.
- **GET /google**: Start Google OAuth authentication.
- **GET /google/callback**: Handle Google OAuth callback and login.
- **GET /logout**: Logout and clear JWT cookies.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
