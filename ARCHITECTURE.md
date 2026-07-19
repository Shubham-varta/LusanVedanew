# ARCHITECTURE.md

# LusanaVeda Architecture

## Overview

LusanaVeda is an AI-powered School Management System built using modern full-stack web technologies.

The project follows a modular architecture to maximize maintainability, scalability, and code reuse.

The codebase should remain clean and beginner-friendly.

---

# Architecture Principles

Always:

- Prefer composition over duplication.
- Keep components reusable.
- Keep business logic separate from UI.
- Keep server logic separate from client logic.
- Keep code readable.
- Minimize dependencies.
- Use TypeScript everywhere.

---

# Technology Stack

Frontend

- Next.js 15 (App Router)
- React
- TypeScript
- Tailwind CSS

Backend

- Next.js Server Actions
- Prisma ORM

Database

Development

- SQLite

Production

- Supabase PostgreSQL

AI

- Google AI Studio (Gemini API)

Deployment

- Vercel

---

# Project Structure

```
app/
components/
lib/
prisma/
public/
types/
hooks/
styles/
```

Only create new top-level folders if absolutely necessary.

---

# App Folder

The App Router contains pages and layouts.

Example

```
app/
│
├── dashboard/
├── students/
├── teachers/
├── attendance/
├── examinations/
├── marks/
├── settings/
├── ai-upload/
└── layout.tsx
```

Each feature should own its page.

---

# Components Folder

Components must be reusable.

Example

```
components/

ui/

dashboard/

students/

teachers/

attendance/

marks/

forms/

tables/

charts/

layout/
```

Never place page-specific logic inside reusable UI components.

---

# Prisma

Database schema belongs only inside

```
prisma/schema.prisma
```

Never duplicate database models.

Always update Prisma using migrations.

---

# Database Design

Primary entities

- Student
- Teacher
- Class
- Section
- Subject
- Attendance
- Examination
- Marks

Relationships should be normalized.

Avoid duplicated information.

---

# Student

Contains

- Personal information
- Roll number
- Class
- Section
- Parent information

Student marks belong in the Marks table.

Attendance belongs in Attendance.

---

# Teacher

Contains

- Personal information
- Contact details
- Assigned subjects
- Assigned classes

---

# Attendance

Separate tables

Student Attendance

Teacher Attendance

Never mix both.

---

# Marks

Each record represents

Student

+

Subject

+

Exam

+

Marks

Avoid storing calculated values.

Compute averages dynamically.

---

# AI Module

Responsible only for

- Upload
- Image processing
- Gemini communication
- JSON validation

The AI module must NOT directly modify the database.

Database updates occur only after teacher approval.

---

# API Design

Prefer

Next.js Server Actions

Use API routes only when necessary.

Keep endpoints focused.

Never create large monolithic endpoints.

---

# State Management

Prefer

- React State
- Server Components
- URL parameters

Avoid introducing Redux, Zustand, MobX, or other global state libraries unless explicitly approved.

---

# Styling

Use Tailwind CSS.

Avoid inline styles.

Keep spacing consistent.

Reuse utility classes.

Use responsive layouts.

---

# Naming Conventions

Components

PascalCase

Example

```
StudentCard.tsx
AttendanceTable.tsx
```

Functions

camelCase

```
calculateAverage()

uploadMarksheet()
```

Variables

camelCase

Constants

UPPER_SNAKE_CASE

Database models

PascalCase

---

# File Size

Aim for

Component

<300 lines

Page

<500 lines

Split large files into smaller reusable components.

---

# Error Handling

Every feature should include

- Loading state
- Empty state
- Error state
- Success notification

Never silently ignore errors.

---

# Validation

Always validate

- User input
- AI output
- Database writes

Never trust external data.

---

# Performance

Always

- Lazy load large components
- Optimize images
- Minimize database queries
- Reuse components
- Avoid unnecessary re-renders

---

# Accessibility

Every page should support

- Keyboard navigation
- Labels
- Focus states
- Proper contrast

---

# Security

Never expose

- API keys
- Secrets
- Database credentials

Use environment variables.

Validate server actions.

---

# Logging

Development

Meaningful console logs are acceptable.

Production

Avoid unnecessary logging.

---

# Testing

Before completing any feature verify

- Application builds
- No obvious TypeScript errors
- No obvious runtime errors
- Feature works
- Existing functionality still works

---

# Git Workflow

After each completed phase

- Explain modified files
- Suggest commit message
- Never commit automatically
- Never push automatically

---

# Development Rules

Always

- Read AGENTS.md
- Read GOAL.md
- Read ROADMAP.md
- Understand the existing code before making changes
- Modify the minimum number of files
- Preserve architecture
- Preserve UI consistency

Never

- Rewrite completed modules
- Delete working code
- Rename folders without approval
- Introduce unnecessary dependencies
- Implement features outside the roadmap

---

# Definition of Good Code

Good code is

- Readable
- Maintainable
- Modular
- Consistent
- Efficient
- Well documented
- Easy for beginners to understand

Every implementation should prioritize simplicity and reliability over cleverness.
