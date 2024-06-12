# TO-DO App with MongoDB

A simple TO-DO application built with Express.js, MongoDB, and Mongoose.

## Features

- Create, update, complete, and delete tasks
- View all tasks

## Prerequisites

- [Node.js](https://nodejs.org/) (v14.x or later)
- [npm](https://www.npmjs.com/) (v6.x or later)
- [MongoDB](https://www.mongodb.com/) (v4.x or later)

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/KamTheCreator/TO-DO-using-MongoDB.git
    cd TO-DO-using-MongoDB
    ```

2. **Install dependencies:**
    ```bash
    npm install
    ```

3. **Set up environment variables:**
    Create a `.env` file with:
    ```
    PORT=3000
    db_connection=mongodb://localhost:27017/todo-app
    ```

## Running the App

1. **Start the server:**
    ```bash
    npm start
    ```

2. **Open in browser:**
    ```
    http://localhost:3000
    ```

## Endpoints

- **GET /**: View all tasks
- **POST /tasks/**: Create a task
- **POST /tasks/:id/complete**: Toggle task completion
- **POST /tasks/:id/update**: Update a task
- **POST /tasks/:id/delete**: Delete a task

## Logging

This application uses `morgan` for logging HTTP requests. Logs will be displayed in the console.

## Static Files

Static files (such as CSS and client-side JavaScript) are served from the `public` directory.

## Views

This application uses EJS for server-side rendering. The views are located in the `views` directory.

## Models

### TaskModel

The `TaskModel` defines the schema for the tasks. It includes the following fields:
- `task` (String): The task content.
- `is_completed` (Boolean): The completion status of the task.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

