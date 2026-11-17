# MT-01 Lab Exam - Vehicle Management System

This repository contains the Vehicle Management Application built using Node.js and Express.js.

## Project Structure

```
Mt-01-LAB-EXAM/
├── VehicleManagement/
│   ├── public/
│   │   └── info.html
│   ├── expressApp.js
│   ├── httpServer.js
│   ├── package.json
│   └── package-lock.json
├── .gitignore
└── README.md
```

## Setup & Installation

1. Navigate to the `VehicleManagement` directory:
   ```bash
   cd VehicleManagement
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Running the Applications

### 1. HTTP Server (Core Node.js)
Runs a custom HTTP server without frameworks using the native `http` module:
```bash
npm run http
```
- Port: `3000` (`http://localhost:3000`)
- Routes:
  - `GET /`: Welcome message
  - `GET /vehicles`: List all vehicles (JSON)
  - `GET /about`: Application info text
  - `GET /info`: Serves static `info.html`
  - `POST /add-vehicle`: Add a new vehicle

### 2. Express Server (REST API)
Runs the Express.js application with full CRUD support:
```bash
npm run express
```
- Port: `4000` (`http://localhost:4000`)
- Routes:
  - `GET /vehicles`: Retrieve all vehicles
  - `GET /vehicles/:id`: Retrieve vehicle by ID
  - `POST /vehicles`: Add a new vehicle
  - `PUT /vehicles/:id`: Update vehicle details
  - `DELETE /vehicles/:id`: Delete vehicle by ID
