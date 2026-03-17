# Todo Frontend (React)

This directory contains the React frontend for a simple todo application. It is a single page app that supports adding, listing, completing/uncompleting, and deleting todos, with persistence in browser storage.

## Features

This frontend implements:

- Adding new todos
- Viewing a list of todos
- Toggling complete/incomplete state
- Deleting todos
- Persistence via browser storage (no backend required)

## Getting Started

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm start
```

Then open:

- http://localhost:3000

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in development mode and serves it on port 3000 by default.

### `npm test`

Runs the test runner (Create React App default behavior is interactive watch mode).

### `npm run build`

Builds the app for production to the `build` folder.

## Configuration

If you want to configure environment-specific values, you can create a `.env` file in this directory and set `REACT_APP_*` environment variables.

The container environment supports the following variables:

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

## Learn More

To learn React, see the React documentation:

- https://reactjs.org/
