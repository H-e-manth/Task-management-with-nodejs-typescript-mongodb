# Task Management System

A **Task Management System** built with **Node.js**, **TypeScript**, and **MongoDB**, providing features like task creation, updating, deletion, and more.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Usage](#usage)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication (JWT-based)
- Create, update, and delete tasks
- Mark tasks as completed
- Filter tasks (by status, priority, etc.)
- Pagination for task listing
- RESTful API structure
- Error handling and validation

## Installation

### Prerequisites

- [Node.js](https://nodejs.org/) (v14.x or higher)
- [MongoDB](https://www.mongodb.com/) (local instance or Atlas)

### Steps

1. Navigate to the project directory:

   ```bash
   cd Task-management-with-nodejs-typescript-mongodb

2. Install the dependencies::

   ```bash
   npm install

3. Create a .env file in the root directory and configure your environment variables:

   ```bash
   PORT=3000 /n MONGODB_URI=mongodb://localhost:27017/taskdb /n JWT_SECRET=your_jwt_secret

4. Start the server:

   ```bash
   npm run dev
   
5.The API will be running at http://localhost:3000.

Technologies Used

> Node.js: JavaScript runtime environment
> TypeScript: Typed superset of JavaScript
> Express.js: Web framework for Node.js
> MongoDB: NoSQL database for data storage
> Mongoose: ODM (Object Data Modeling) library for MongoDB and Node.js
> JWT: JSON Web Tokens for authentication
> ESLint: Linting utility for JavaScript/TypeScript
> Prettier: Code formatting tool

API Endpoints

Authentication

POST /api/auth/signup: Register a new user
POST /api/auth/login: Authenticate and get a token

Tasks

GET /api/tasks: Get all tasks (with optional filters and pagination)
POST /api/tasks: Create a new task
PUT /api/tasks/:id: Update a task
DELETE /api/tasks/:id: Delete a task
PATCH /api/tasks/:id/complete: Mark a task as completed


Example Request
 ```bash
POST /api/tasks
Content-Type: application/json
Authorization: Bearer <token>

{
  "title": "Finish the report",
  "description": "Complete the quarterly financial report",
  "priority": "High",
  "dueDate": "2024-10-10"
}







