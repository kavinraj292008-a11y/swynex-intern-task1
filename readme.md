# Node.js Backend Service

A simple backend service built using **Node.js and Express.js**, featuring a health-check API endpoint and environment-based configuration.

## Features

- Health-check endpoint (`GET /health`)
- Environment configuration using dotenv
- Modular project structure
- JSON response handling
- Automatic server restart using Nodemon

## Tech Stack

- Node.js
- Express.js
- dotenv
- Nodemon

## Project Structure

```text
node-backend/
├── src/
│   ├── routes/
│   │   └── health.routes.js
│   ├── controllers/
│   │   └── health.controller.js
│   └── server.js
├── .env
├── .gitignore
└── package.json
```

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Navigate to the project directory:

```bash
cd node-backend
```

3. Install dependencies:

```bash
npm install
```

4. Create a `.env` file:

```env
PORT=3000
NODE_ENV=development
```

## Run the Project

Start the development server:

```bash
npm run dev
```

For production mode:

```bash
npm start
```

The server will run at:

`http://localhost:3000`

## API Endpoint

### Health Check

| Method | Endpoint | Description |
|---|---|---|
| GET | `/health` | Checks server availability |

**Sample Response:**

```json
{
  "success": true,
  "message": "Server is running",
  "timestamp": "2026-11-24T..."
}
```

## Learning Objectives

- Understanding Node.js backend development
- Building REST API endpoints with Express.js
- Managing environment variables
- Organizing backend code using routes and controllers

## Author

Kavin Raj A.

---

Built as part of my backend development learning journey.