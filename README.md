# ATHAR — أَثَر

ATHAR is a responsive educational-platform frontend concept for preparatory and secondary students. Its bilingual Arabic/English experience supports RTL and LTR layouts.

## Run locally

Requirements: Node.js 18 or later.

```bash
npm install
npm run dev
```

Create a production build with:

```bash
npm run build
```

## Frontend demo

- Student, parent, and admin demo entry points.
- Student registration flow with school-system and grade selection, followed by a simulated subscription checkout.
- Student dashboard, subjects, chapter summary, search, notifications, achievements, progress, and subscription screens.
- Timed quizzes with exactly 10 multiple-choice questions, scoring, answer review, and explanations.
- Admin content and account-management screens.
- Demo preferences and selected progress counters persisted in browser `localStorage`.
- Screenshot-related warnings are deterrents only; browsers cannot reliably prevent screenshots.

## Integration status

This repository currently contains a frontend demo with sample data. Authentication, role-based authorization, payment processing, content management, and progress persistence are not backed by a server. The checkout does not charge a payment method or verify a provider transaction. Do not use the demo to collect real credentials or payment details.

Before production, integrate a backend for authentication and authorization, server-enforced subscription checks, protected content delivery, validated quiz results, and a payment provider that confirms transactions server-side. Never store raw card details or commit secrets. Configure any future credentials through environment variables and keep local `.env` files out of version control.

## Stack

- React and TypeScript
- Vite
- Tailwind CSS
- Framer Motion
- Lucide React
