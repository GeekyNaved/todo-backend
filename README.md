# Todo App

A basic CRUD Todo application using Node.js, Express.js, and MongoDB.

## Features
- Create, Read, Update, and Delete todos
- RESTful API
- MongoDB with Mongoose
- Error handling middleware
- Environment variable support

## Project Structure
```
todo-app/
├── config/                   # Database configuration
│   └── db.js
├── controllers/              # CRUD operations
│   └── todoController.js
├── models/                   # Mongoose schema
│   └── todoModel.js
├── routes/                   # API routes
│   └── todoRoutes.js
├── middleware/               # Error handling
│   └── errorMiddleware.js
├── .env                      # Environment variables
├── package.json              # Project dependencies and scripts
├── app.js                 # Main entry point
└── README.md                 # Project documentation
```

## Getting Started

### Prerequisites
- Node.js
- MongoDB

### Installation
1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the root directory and add:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/todoapp
   ```
4. Start the server:
   ```bash
   npm start
   ```

## API Endpoints
| Method | Endpoint         | Description         |
|--------|------------------|--------------------|
| GET    | /api/todos       | Get all todos      |
| POST   | /api/todos       | Create a new todo  |
| PUT    | /api/todos/:id   | Update a todo      |
| DELETE | /api/todos/:id   | Delete a todo      |

### Sample Todo Model
```
title: String (required)
description: String (optional)
completed: Boolean (default: false)
```

## Error Handling
- 404 Not Found middleware
- General error handler middleware

## License
ISC 