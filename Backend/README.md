# Blog App Backend

This is the backend for a beautiful MERN stack blog application. It provides a RESTful API for blog posts, user authentication, and media uploads.

## Features

- User authentication (register, login, JWT)
- Post CRUD operations
- Comments and likes on posts
- User profiles
- Image uploads for posts and user profiles
- Pagination, filtering, and search functionality

## Tech Stack

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Multer for file uploads

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user

### Posts
- `GET /api/posts` - Get all posts (with pagination, filtering, search)
- `GET /api/posts/:id` - Get a single post
- `POST /api/posts` - Create a new post (auth required)
- `PUT /api/posts/:id` - Update a post (auth required)
- `DELETE /api/posts/:id` - Delete a post (auth required)
- `POST /api/posts/:id/comments` - Add a comment (auth required)
- `DELETE /api/posts/:id/comments/:commentId` - Delete a comment (auth required)
- `PUT /api/posts/:id/like` - Like/unlike a post (auth required)

### Users
- `PUT /api/users/profile` - Update user profile (auth required)
- `GET /api/users/:id` - Get user profile
- `GET /api/users/:id/posts` - Get posts by a user

## Getting Started

1. Install dependencies:
   ```
   npm install
   ```

2. Create a `.env` file with:
   ```
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   NODE_ENV=development
   ```

3. Run the server:
   ```
   npm run dev
   ``` 