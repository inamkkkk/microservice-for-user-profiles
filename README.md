# User Profile Microservice

A Node.js microservice for managing user profiles, including registration, login, and user data management.

## Features

-   User registration and authentication using JWT
-   User profile management (CRUD operations)
-   MongoDB database integration
-   Error handling and logging
-   Well-structured project with multiple folders

## Technologies Used

-   Node.js
-   Express.js
-   MongoDB
-   Mongoose
-   JWT (JSON Web Tokens)
-   bcryptjs
-   cors

## Getting Started

1.  Clone the repository:
    
    
    git clone <repository_url>
    
2.  Install dependencies:
    
    
    npm install
    
3.  Configure environment variables:
    
    Create a `.env` file in the root directory and add the following variables:
    
    
    PORT=3000
    DB_URL=mongodb://localhost:27017/userProfiles
    JWT_SECRET=secretKey
    
    
    Replace the values with your desired configuration.

4.  Run the application:
    
    
    node server.js
    

## API Endpoints

### Authentication

-   `POST /auth/register`: Register a new user.
-   `POST /auth/login`: Login an existing user.

### User Management

-   `GET /users`: Get all users (requires authentication).
-   `GET /users/:id`: Get a specific user by ID (requires authentication).
-   `POST /users`: Create a new user (requires authentication).
-   `PUT /users/:id`: Update a user (requires authentication).
-   `DELETE /users/:id`: Delete a user (requires authentication).
