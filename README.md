# Task Tracking Database

## Overview

Task Tracking Database is a backend application built using **Node.js**, **Express.js**, **MongoDB**, and **Mongoose**. It helps manage and track tasks by allowing users to create, view, update, and delete task records.

This project demonstrates CRUD operations and database integration commonly used in real-world task management systems.

---

## Features

* Create new tasks
* View all tasks
* Get task details by ID
* Update task information
* Delete tasks
* Store task status and priority
* MongoDB database integration

---

## Technologies Used

* Node.js
* Express.js
* MongoDB
* Mongoose
* Postman
* dotenv

---

## Project Structure

```text
TaskTrackingDatabase
│
├── models
│   └── Task.js
│
├── routes
│   └── taskRoutes.js
│
├── .env
├── server.js
├── package.json
└── README.md
```

## Database Schema

Each task contains:

| Field       | Description                       |
| ----------- | --------------------------------- |
| taskId      | Unique Task ID                    |
| title       | Task Title                        |
| description | Task Description                  |
| assignedTo  | Assigned Person                   |
| priority    | Low / Medium / High               |
| status      | Pending / In Progress / Completed |
| dueDate     | Task Deadline                     |

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd TaskTrackingDatabase
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/taskDB
```

### Run Server

```bash
npm run dev
```

Server Output:

```text
MongoDB Connected
Server running on port 5000
```

---

## API Endpoints

### Create Task

```http
POST /api/tasks
```

### Get All Tasks

```http
GET /api/tasks
```

### Get Task By ID

```http
GET /api/tasks/:id
```

### Update Task

```http
PUT /api/tasks/:id
```

### Delete Task

```http
DELETE /api/tasks/:id

---

## Testing

All APIs were tested using Postman and verified in MongoDB Compass.

### Verified Operations

* Create Task
* Read Tasks
* Update Task
* Delete Task
---

a MongoDB Backend Development Internship Task.
