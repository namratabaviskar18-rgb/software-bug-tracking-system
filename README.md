# Software Bug Reporting & Tracking System

A web application for reporting software bugs, tracking issue status, and organizing bug fixes. The interface is built with React, TypeScript, and TanStack Start. Supabase is used for backend data and authentication integration.

## Features
- View and track reported bugs
- Record bug severity and status
- Organize bug reports in one place

## Technology Stack
- React + TypeScript
- TanStack Start and TanStack Router
- Tailwind CSS
- Supabase
- Drizzle ORM / SQL migrations
- Vite

## Run locally
1. Install Node.js (LTS) from https://nodejs.org/
2. Open a terminal in this project folder.
3. Run `npm install`
4. Set the required Supabase environment variables in your hosting provider or local environment. The app expects `VITE_SUPABASE_URL` and `VITE_SUPABASE_PUBLISHABLE_KEY` for the browser client; server features may also require `SUPABASE_URL` and server-only keys. Never expose a Supabase service-role key in browser code or commit it to GitHub.
5. Run `npm run dev` to start the development server.

## Build
Run `npm run build` to create a production build.

## Deployment note
The source code can be hosted on a platform that supports TanStack Start/Vite. To make bug reports persist online, configure the Supabase project and database using the SQL migration in `drizzle/migrations/`. A successful website deployment alone does not configure the database.
