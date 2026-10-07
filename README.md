# Kambaz (Next.js)

A Canvas-style learning management interface built with Next.js, React, and React Bootstrap for Northeastern's Web Development course. It has the app shell and page layouts: account pages, a course dashboard, and course pages for modules, assignments, and people.

## Tech stack

- Next.js 15 (App Router, Turbopack)
- React 19 + TypeScript
- React Bootstrap / Bootstrap 5
- React Icons
- Tailwind CSS 4 (PostCSS setup)

## Features

- **Global sidebar navigation:** Account, Dashboard, Courses, Calendar, Inbox, and Labs
- **Account:** Sign in, Sign up, and Profile pages, with their own account navigation
- **Dashboard:** a responsive grid of course cards
- **Course pages** (dynamic `/Courses/[cid]` routes) with course navigation:
  - Home (modules and a course status panel)
  - Modules (with lesson controls)
  - Assignments list and an assignment editor (`/Assignments/[aid]`)
  - People table
  - Placeholder pages for Grades, Quizzes, Piazza, and Zoom
- **Labs:** exercises on Bootstrap grids, flexbox, positioning, forms, tables, lists, navigation, and React Icons

The UI currently uses static, hard-coded content. The matching REST backend lives in a separate repo (see below).

## Getting started

```bash
npm install
npm run dev      # start the dev server at http://localhost:3000
npm run build    # production build
npm start        # serve the production build
npm run lint
```

## Project structure

```
app/
  (kambaz)/
    Navigation.tsx          # Main sidebar
    Account/                # Signin, Signup, Profile
    Dashboard/              # Course cards
    Courses/[cid]/          # Home, Modules, Assignments, People, Grades, ...
    Calendar/, Inbox/
  Labs/                     # Lab1-Lab3 exercises
public/images/              # Course and logo images
```

## Related

- Backend: [kambaz-node-server-app](https://github.com/NithishBhat/kambaz-node-server-app) (Node.js + Express REST API)
