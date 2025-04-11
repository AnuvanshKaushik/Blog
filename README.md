# Blog App Frontend

This is the frontend for a beautiful MERN stack blog application. It provides a modern UI for reading and writing blog posts.

## Features

- User authentication (register, login)
- Responsive design
- Blog post listing and details
- Create and edit posts
- Comment on posts
- Like posts
- User profiles

## Tech Stack

- React with TypeScript
- React Router for navigation
- Context API for state management
- Tailwind CSS for styling
- Axios for API requests

## Getting Started

1. Install dependencies:
   ```
   npm install
   ```

2. Start the development server:
   ```
   npm run dev
   ```

3. Build for production:
   ```
   npm run build
   ```

## Project Structure

- `/src/api` - API configuration and utilities
- `/src/components` - Reusable UI components
- `/src/context` - Context providers for state management
- `/src/hooks` - Custom React hooks
- `/src/pages` - Page-level components
- `/src/types` - TypeScript type definitions
- `/src/utils` - Utility functions

## Required Environment

Make sure the backend server is running on `http://localhost:5000`. If your backend is running on a different URL, update the `baseURL` in `/src/api/axios.ts`.
