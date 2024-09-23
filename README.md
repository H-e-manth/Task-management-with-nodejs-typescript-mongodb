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

2.Install the dependencies:

  ```bash
 npm install


PORT=3000
MONGODB_URI=mongodb://localhost:27017/taskdb
JWT_SECRET=your_jwt_secret


npm run dev
