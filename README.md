# Student Management System (MVC + MongoDB + Node.js)

## Overview
This is a simple MVC-based REST API built using Node.js, Express, and MongoDB (via Mongoose).
It allows managing student records with CRUD operations.

## Folder Structure
```
├── controllers/
│   └── studentController.js
├── models/
│   └── Student.js
├── routes/
│   └── studentRoutes.js
├── server.js
├── .env.example
├── package.json
└── README.md
```

## Setup
1. Clone or extract this project.
2. Copy `.env.example` to `.env` and edit MongoDB URI if needed.
3. Install dependencies:
   ```bash
   npm install
   ```
4. Run the server:
   ```bash
   npm run dev
   ```
   or
   ```bash
   npm start
   ```

## API Endpoints
| Method | Endpoint | Description |
|---------|-----------|-------------|
| GET | /students | Get all students |
| GET | /students/:id | Get student by ID |
| POST | /students | Create a student |
| PUT | /students/:id | Update a student |
| DELETE | /students/:id | Delete a student |

## Example MongoDB Document
```json
{
  "_id": "60f5f66da1801707c14d09e60",
  "name": "Alice Johnson",
  "age": 20,
  "course": "Computer Science"
}
```

## Notes
- Built using MVC structure for clean separation of concerns.
- Includes validation and error handling.
