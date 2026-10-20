# Kambaz

Live site: https://kambaz-next-js-zeta-seven.vercel.app

Kambaz is a Canvas-style learning management system I built for the Web Development course at Northeastern. This repo is the Next.js frontend. The backend is [kambaz-node-server-app](https://github.com/NithishBhat/kambaz-node-server-app) (Express + MongoDB, hosted on Render).

## Features

- Sign up, sign in and profile editing with cookie-based sessions
- Role-based views for students, faculty and admins
- Dashboard of enrolled courses; faculty can create, edit and delete courses, students can enroll and unenroll
- Course modules and assignments with full create/edit/delete for faculty
- People page with user details and role editing
- Quizzes:
  - Faculty editor for quiz settings (time limit, multiple attempts, shuffle answers, access code, one question at a time, due/available dates, publish)
  - Question editor for multiple choice, true/false and fill-in-the-blank questions
  - Preview mode and student attempts with scoring and attempt history

## Stack

Next.js (App Router), React 19, TypeScript, Redux Toolkit, Axios, React Bootstrap

## Running locally

```bash
npm install
npm run dev      # http://localhost:3000
```

By default the app talks to `http://localhost:4000`. To point it somewhere else, set `NEXT_PUBLIC_HTTP_SERVER` in `.env.local`. Production builds use the Render URL in `.env.production`.
