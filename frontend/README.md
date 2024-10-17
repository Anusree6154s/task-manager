# Task Manager

A full-stack Task Manager application built with React on the frontend and Node.js with Express on the backend. This application allows users to create, edit, delete, and manage tasks, along with file uploads associated with tasks.

## Table of Contents

- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [API Endpoints](#api-endpoints)

## Setup and Installation

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (locally or via a cloud service like MongoDB Atlas)

### Steps to Set Up the Backend

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Anusree6154s/task-manager.git
   cd taskManager/backend
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Create a `.env` file** in the `backend` folder and add your MongoDB URI:

   ```plaintext
   MONGO_URI=<your_mongodb_uri>
   ```

4. **Start the server**:

   ```bash
   node server.js
   ```

### Steps to Set Up the Frontend

1. **Navigate to the frontend directory**:

   ```bash
   cd taskManager/frontend
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Start the development server**:

   ```bash
   npm start
   ```

## Usage

- Open your browser and go to `http://localhost:3000` for the frontend.
- The backend will be running on `http://localhost:8082`.
- You can create tasks, upload files, mark tasks as done, and delete tasks through the user interface.

## Features

- Create, read, update, and delete tasks.
- Upload and link files to tasks.
- Mark tasks as done.
- Responsive design with Material-UI components.
- User-friendly interface for managing tasks.

## Technologies Used

- **Frontend**:

  - React
  - Material-UI
  - Axios (for API calls)

- **Backend**:
  - Node.js
  - Express
  - MongoDB (using Mongoose)
  - Multer (for file uploads)
  - dotenv (for environment variables)

## API Endpoints

| Method | Endpoint     | Description             |
| ------ | ------------ | ----------------------- |
| GET    | `/tasks`     | Retrieve all tasks      |
| POST   | `/tasks`     | Create a new task       |
| PATCH  | `/tasks/:id` | Update an existing task |
| DELETE | `/tasks/:id` | Delete a task           |
