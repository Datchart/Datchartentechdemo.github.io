# Frontend Application

This directory contains the standalone frontend application for the DatchCode Portfolio project. It's a modern single-page application built with Angular (v20+), featuring a zoneless change detection strategy for high performance.

## Features

-   **Modern Angular:** Built with the latest Angular features, including Standalone Components and Signals for state management.
-   **Zoneless:** Optimized for performance by running without Zone.js.
-   **Responsive Design:** Fully responsive and beautifully designed with Tailwind CSS.
-   **Dynamic Content:** Fetches all project and message data from the backend API.
-   **AI Chat:** Includes an interactive, draggable AI chat assistant that streams responses from the backend.
-   **Decoupled:** Can be configured to connect to any compatible backend API.

## Tech Stack

-   **[Angular](https://angular.io/)** (v20+)
    -   Standalone Components
    -   Signals for state management
    -   Zoneless Change Detection
-   **[Tailwind CSS](https://tailwindcss.com/)**: For styling.
-   **[TypeScript](https://www.typescriptlang.org/)**: For type safety.

## Getting Started

### 1. Prerequisites

This project is designed to be run without a complex build setup. All you need is a simple local HTTP server. You can use any server you like, but `http-server` is a great, simple option.

If you don't have `http-server`, you can install it globally via npm:
```bash
npm install -g http-server
```

### 2. Configure the API Endpoint (Optional)

The frontend is configured to connect to the backend API at `http://localhost:3000/api` by default.

If your backend is running on a different address, you can change the `API_BASE_URL` constant in the following file:
`frontend/src/app/config.ts`

### 3. Run the Development Server

Navigate to the `frontend` directory and start your HTTP server.

```bash
cd frontend
http-server -c-1
```
The `-c-1` flag disables caching, which is useful for development.

The application will now be available at `http://localhost:8080`.

**Note:** For the application to function correctly, the backend server must be running at the same time.
