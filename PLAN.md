# Quiz Forge - Project Plan

## 1. Assumptions & Tech Stack
- **Framework**: Next.js 14 (App Router)
- **Database**: Neon via Prisma
- **Package Manager**: pnpm
- **Styling**: Tailwind CSS + Shadcn UI

## 2. Scope
- **Admin**: Create Quiz (form), List Quizzes.
- **Public**: Take Quiz (Dynamic ID), view Results (Score).

## 3. Database Schema (Draft)
- `Quiz` (id, title, description, createdAt, updatedAt)
- `Question` (id, quizId, q_text, q_type, q_options, correctAnswer, createdAt, updatedAt)
- `Attempt` (id, quizId, score, createdAt, updatedAt)

## 4. Trade-offs
- **Monorepo**: Using a single monorepo for velocity and ease of development.
- **Server Actions**: Using simple "Server Action" instead of a separate API backend to save time.
