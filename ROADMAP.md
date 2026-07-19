# ROADMAP.md

# LusanaVeda Development Roadmap

This document defines the official implementation order for LusanaVeda.

The implementation order must not be changed unless explicitly approved.

Always complete one phase completely before beginning the next.

Never implement multiple phases simultaneously.

---

# General Rules

Before every phase:

- Read AGENTS.md.
- Read GOAL.md.
- Understand the current repository.
- Verify previous phases are complete.

After every phase:

- Verify the application builds.
- Verify existing features still work.
- Verify UI consistency.
- Explain all modified files.
- Explain commands to run.
- Suggest a Git commit message.
- Stop and wait for approval.

---

# Phase 1 — Project Foundation

Objective

Establish a clean project foundation.

Tasks

- Verify Next.js setup
- Verify Tailwind CSS
- Verify TypeScript
- Configure Prisma
- Configure SQLite
- Configure project structure
- Verify linting
- Verify formatting

Deliverable

A stable project foundation.

---

# Phase 2 — Core Layout

Objective

Build the application's base UI.

Tasks

- Sidebar
- Top Navigation
- Dashboard Layout
- Routing
- Theme
- Global styles
- Responsive layout

Deliverable

Professional application shell.

---

# Phase 3 — Core Data Modules

Objective

Implement school management modules.

Tasks

Student Management

- List
- Add
- Edit
- Delete
- Search
- Filters

Teacher Management

- List
- Add
- Edit
- Delete

Class Management

Subject Management

Deliverable

Core CRUD modules.

---

# Phase 4 — Attendance

Objective

Implement attendance management.

Student Attendance

- Present
- Absent
- Late

Teacher Attendance

- Present
- Absent
- Leave

Features

- Daily attendance
- Attendance history
- Attendance percentage
- Dashboard summaries
- Search
- Filters

Deliverable

Complete attendance module.

---

# Phase 5 — Examination System

Objective

Create examination management.

Tasks

- Exams
- Subjects
- Maximum marks
- Edit exams
- Delete exams
- Search

Deliverable

Functional examination system.

---

# Phase 6 — Marks Management

Objective

Manage student marks.

Tasks

- Marks table
- Subject marks
- Edit marks
- Delete marks
- Student academic history
- Search

Deliverable

Working marks module.

---

# Phase 7 — AI Marksheet Upload

Highest Priority

Objective

Implement the complete AI workflow.

Tasks

- Upload image
- Preview image
- Send image to Gemini API
- Extract structured JSON
- Validate extracted data
- Confidence checking
- Error detection

Deliverable

AI successfully extracts student marks.

---

# Phase 8 — AI Review Screen

Objective

Allow teacher verification.

Tasks

- Editable table
- Edit rows
- Delete rows
- Add rows
- Validation
- Approve import

Deliverable

Teacher-controlled AI review.

---

# Phase 9 — Automatic Import

Objective

Automatically update records.

Tasks

- Update students
- Update marks
- Refresh dashboard
- Refresh profiles
- Success notifications

Deliverable

Complete import workflow.

---

# Phase 10 — Dashboard Intelligence

Objective

Improve analytics.

Tasks

Dashboard cards

Charts

Statistics

Attendance summaries

Recent activity

Quick actions

AI Performance Summary

Generate:

- Average marks
- Highest marks
- Lowest marks
- Students requiring attention

Deliverable

Professional dashboard.

---

# Phase 11 — Search & Settings

Objective

Complete utility features.

Tasks

Global Search

Search:

- Students
- Teachers
- Subjects
- Classes

Settings

- School name
- Academic year
- Logo

Deliverable

Complete utility module.

---

# Phase 12 — Polish

Objective

Prepare hackathon submission.

Tasks

- Improve responsiveness
- Improve accessibility
- Improve loading states
- Improve empty states
- Improve error handling
- Fix TypeScript issues
- Fix lint warnings
- Improve animations
- Improve UX

Deliverable

Production-quality MVP.

---

# Out of Scope

Do NOT implement

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
- Library
- Inventory
- Payroll
- Multi-school Support

---

# Development Principles

Always

- Build one phase only.
- Keep changes small.
- Preserve architecture.
- Preserve UI.
- Reuse components.
- Use TypeScript.
- Use Prisma.
- Use SQLite during development.
- Write maintainable code.

Never

- Rewrite completed features.
- Refactor unrelated code.
- Introduce unnecessary dependencies.
- Break existing functionality.

---

# Completion Criteria

The project is complete when:

✓ All phases are implemented.

✓ The application builds successfully.

✓ No obvious TypeScript errors remain.

✓ Existing functionality works.

✓ The AI workflow is fully demonstrable.

✓ The UI is polished.

✓ The project is ready for deployment to Vercel using Supabase PostgreSQL.
