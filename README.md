# Dockerized Full Stack Application

A simple Dockerized full-stack task manager application with a static frontend, a Node.js backend, and a MongoDB database. The project follows a multi-container setup where each service runs in its own container and communicates over a shared Docker network.

## Project overview

This project is based on a walkthrough that demonstrates how to build a full-stack app using Docker, with Nginx serving the frontend, Node.js handling the backend API, and MongoDB storing task data. The application allows users to add tasks and view existing tasks through API calls between the frontend and backend.

## Tech stack

- Frontend: Static HTML/JavaScript served with Nginx.
- Backend: Node.js with Express for API routes.
- Database: MongoDB with Mongoose for data modeling and persistence.
- Container orchestration: Docker with a multi-container workflow and shared networking.

## Features

- Add and view tasks in a simple task manager interface.
- Run frontend, backend, and database in isolated containers.
- Connect services through Docker networking.
- Persist and retrieve task data through MongoDB.

## How it works

1. The frontend sends HTTP requests to the backend API running on port 3000.
2. The backend exposes routes for fetching tasks and creating new tasks.
3. The backend connects to MongoDB using Mongoose to store and retrieve task records.
4. Docker isolates each component in its own container so the full application can run consistently across environments.
