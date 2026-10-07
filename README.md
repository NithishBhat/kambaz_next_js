# Kambaz (Next.js frontend)

Kambaz is a course-management website modeled on Canvas, the system Northeastern students use to find course materials, assignments and grades. I built this frontend for my Web Development course at Northeastern. It covers the main screens a student sees: signing in, a dashboard of enrolled courses, and per-course pages for modules, assignments and the class roster.

It's a work in progress. Every page currently renders hard-coded sample content, and the frontend isn't connected yet to the backend API I wrote for it ([kambaz-node-server-app](https://github.com/NithishBhat/kambaz-node-server-app)). Grades, Quizzes, Piazza and Zoom are placeholder pages.

## What's here

- A left sidebar for Account, Dashboard, Courses, Calendar, Inbox and Labs
- Sign in, sign up and profile pages
- A dashboard with a grid of course cards
- Course pages under `/Courses/[cid]`: Home, Modules, an assignments list with an editor page (`/Assignments/[aid]`), and a People table
- `Labs/`: the weekly course exercises (Bootstrap layout, flexbox, positioning, forms, tables, React Icons)

Built with Next.js 15 (App Router), React 19, TypeScript and React Bootstrap. Tailwind 4 is installed through PostCSS.

## Running it

```bash
npm install
npm run dev      # http://localhost:3000
npm run build
npm start
npm run lint
```

## Layout

```
app/
  (kambaz)/
    Navigation.tsx      sidebar
    Account/            Signin, Signup, Profile
    Dashboard/          course cards
    Courses/[cid]/      Home, Modules, Assignments, People, Grades, ...
    Calendar/, Inbox/
  Labs/                 Lab1-Lab3
public/images/          course and logo images
```
