# Simple Todo Application (React Frontend)

This repository contains a single React frontend container that implements a minimal todo application. The app runs as a client-side single page application and persists todos in browser storage, with no backend service required.

## Features

This application supports the core todo workflow in a clean, minimal UI.

It includes the following features:

- Adding new todos
- Listing existing todos
- Marking a todo as complete or incomplete
- Deleting a todo
- Persisting todos in browser storage (so they remain after refresh)

## Project Structure

The primary application lives in the `todo_frontend/` directory.

- `simple-todo-application-245417-245431/todo_frontend/`: React application (Create React App style project)
- `simple-todo-application-245417-245431/README.md`: This repository-level README

## Prerequisites

You will need a recent Node.js LTS version and npm.

## Setup

Install dependencies from within the frontend container directory.

```bash
cd simple-todo-application-245417-245431/todo_frontend
npm install
```

## Running the App (Development)

Start the development server:

```bash
cd simple-todo-application-245417-245431/todo_frontend
npm start
```

By default, Create React App serves the application at:

- http://localhost:3000

## Scripts

All scripts are run from `todo_frontend/`.

- `npm start` starts the development server.
- `npm test` runs the test runner (interactive by default in CRA).
- `npm run build` creates a production build in `todo_frontend/build/`.

## Configuration (Environment Variables)

This container supports a set of `REACT_APP_*` environment variables (typical for React apps built with Create React App). If you are using a `.env` file, it should be placed in:

- `simple-todo-application-245417-245431/todo_frontend/.env`

The following variables are defined for the container environment:

- `REACT_APP_API_BASE`
- `REACT_APP_BACKEND_URL`
- `REACT_APP_FRONTEND_URL`
- `REACT_APP_WS_URL`
- `REACT_APP_NODE_ENV`
- `REACT_APP_NEXT_TELEMETRY_DISABLED`
- `REACT_APP_ENABLE_SOURCE_MAPS`
- `REACT_APP_PORT`
- `REACT_APP_TRUST_PROXY`
- `REACT_APP_LOG_LEVEL`
- `REACT_APP_HEALTHCHECK_PATH`
- `REACT_APP_FEATURE_FLAGS`
- `REACT_APP_EXPERIMENTS_ENABLED`

If you do not set these variables, the app will still run as a standalone frontend (and will continue to use browser storage for persistence).

## Persistence

Todo items are persisted in browser storage. This means the state is retained across page refreshes in the same browser profile, but it is local to that browser and device.

## Notes

This repository currently contains only the frontend container. No database or backend container is included.
