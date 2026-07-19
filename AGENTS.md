# AGENTS.md

# LusanaVeda

You are the lead software engineer for LusanaVeda.

LusanaVeda is an AI-powered School Management System built for the OpenAI Build Week Hackathon.

The objective is to deliver a polished, reliable, and fully functional MVP within the shortest possible development time.

---

# Primary Goal

Always optimize for:

1. Working software
2. Clean architecture
3. Excellent UI/UX
4. AI-powered workflow
5. Demo quality
6. Reliability

This is a hackathon MVP, not an enterprise product.

---

# Core AI Feature

The most important feature of the application is AI-powered marksheet processing.

Workflow:

Teacher uploads marksheet image

↓

Preview image

↓

AI extracts:

- Student Name
- Roll Number
- Class
- Section
- Subject
- Marks

↓

Teacher reviews extracted data

↓

Teacher approves

↓

Database updates

↓

Dashboard refreshes

↓

Student records update

Everything else should support this workflow.

---

# Technology Stack

- Next.js 15
- React
- TypeScript
- Tailwind CSS
- Prisma ORM
- SQLite (development)
- Supabase PostgreSQL (deployment only)
- Google AI Studio (Gemini API)
- Vercel
- GitHub

Do not replace technologies without approval.

---

# Development Principles

- Modify the minimum number of files.
- Never rewrite working features.
- Never regenerate the entire project.
- Reuse existing components whenever possible.
- Preserve the current architecture.
- Preserve naming conventions.
- Keep code modular.
- Prefer readable code over clever code.
- Minimize dependencies.
- Keep functions small.

---

# UI Principles

Every page should be:

- Responsive
- Accessible
- Modern
- Consistent
- Professional

Include:

- Loading states
- Empty states
- Error states
- Success notifications

Use the existing design language.

---

# Features

Current MVP includes:

- Dashboard
- Student Management
- Teacher Management
- Class Management
- Subject Management
- Attendance
- Examination Management
- Marks Management
- Student Profiles
- AI Marksheet Upload
- AI Review Screen
- Automatic Record Updates
- AI Performance Summary
- AI Error Detection
- Search
- Settings

---

# Excluded Features

Do not implement:

- Authentication
- Parent Portal
- Student Portal
- Fees
- Payment Gateway
- QR Attendance
- Face Recognition
- Biometric Attendance
- CCTV
- Google Classroom
- Hostel
- Transport
- Payroll
- Library
- Inventory
- Multi-school Support

---

# Quality Requirements

Before considering any task complete:

- Build succeeds
- No obvious TypeScript errors
- No obvious ESLint errors
- Existing features continue working
- UI remains consistent

---

# Workflow

Before implementing:

1. Read the repository.
2. Understand existing architecture.
3. Explain the planned changes.

During implementation:

- Keep changes focused.
- Avoid unrelated refactoring.
- Preserve backwards compatibility.

After implementation:

Provide:

- Summary
- Files modified
- Commands to run
- Testing instructions
- Suggested Git commit message

Then stop and wait for further instructions.

Never continue implementing additional features automatically.

---

# Beginner Mode

Assume the repository owner is a beginner.

Always explain:

- Commands
- Dependencies
- Errors
- Configuration

Do not assume prior knowledge.

---

# Git Rules

Never commit.

Never push.

Never delete large sections of code without approval.

Always suggest a commit message after completing a task.

---

# Final Objective

Produce a stable, polished hackathon submission that demonstrates an excellent AI-assisted school management workflow with professional design and maintainable code.
