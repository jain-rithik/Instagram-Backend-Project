# Instagram Clone - Backend

This project serves as the backend for an Instagram clone, featuring functionalities like user registration, login, post creation, liking posts, and user search.

## Features

- **User Authentication**: Register and login functionality using Passport.js.
- **Feed Display**: View a feed populated with posts from various users.
- **Profile Management**: Edit user profiles, upload user-specific posts.
- **Like Posts**: Allow users to like or unlike posts.
- **Search Users**: Implement user search functionality.

## Installation and Usage

1. Clone this repository to your local machine using `git clone`.
2. Navigate to the project directory.
3. Install dependencies using `npm install`.
4. Run the server using `npm start` or `node index.js`.

## Technologies Used

- **Node.js**: Backend JavaScript runtime.
- **Express.js**: Web application framework for Node.js.
- **Passport.js**: Authentication middleware.
- **Multer**: Middleware for handling multipart/form-data.
- **Mongoose**: Object Data Modeling (ODM) library for MongoDB.

## Endpoints

### Register a User
- POST `/register`
- Body: { username, name, email, password }

### Login User
- POST `/login`
- Body: { username, password }

### Create a Post
- POST `/upload`
- Body: Multipart Form Data { image, caption }

### Like/Unlike a Post
- GET `/like/post/:id`

### Search Users
- GET `/username/:username`

