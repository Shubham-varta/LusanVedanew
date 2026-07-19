# GOAL.md

# LusanaVeda - Project Goal

## Mission

Build a polished, AI-powered School Management System that demonstrates how artificial intelligence can automate repetitive school administration tasks while providing an exceptional user experience.

This project is being built as a hackathon MVP for the OpenAI Build Week Hackathon.

The application should feel like a modern production-ready SaaS product while remaining simple enough to complete within the hackathon timeline.

---

# Primary Objective

The application must successfully demonstrate one complete AI workflow from beginning to end.

The primary demonstration flow is:

Teacher uploads a marksheet image

↓

Image preview

↓

AI extracts structured student data

↓

Teacher reviews extracted data

↓

Teacher approves import

↓

Database updates automatically

↓

Dashboard refreshes

↓

Student profiles and marks update automatically

This workflow is the highest priority of the project.

Everything else supports this workflow.

---

# Product Vision

Schools spend significant time entering student records manually.

LusanaVeda eliminates repetitive administrative work by allowing teachers to upload academic documents and letting AI organize the data automatically.

The application should feel intelligent, simple and professional.

---

# Target Users

- Schools
- Teachers
- School Administrators

---

# Design Philosophy

The interface should be:

- Clean
- Modern
- Responsive
- Minimal
- Professional
- Fast
- Easy to understand

Inspired by modern SaaS dashboards.

---

# Technology Stack

Frontend

- Next.js 15
- React
- TypeScript
- Tailwind CSS

Backend

- Next.js Server Actions
- Prisma ORM

Database

- SQLite during development
- Supabase PostgreSQL during deployment

AI

- Google AI Studio (Gemini API)

Deployment

- Vercel

Version Control

- GitHub

---

# MVP Features

## Dashboard

- School statistics
- Charts
- Recent activity
- Quick actions

---

## Student Management

- Student list
- Student profile
- Add student
- Edit student
- Delete student
- Search
- Filter

---

## Teacher Management

- Teacher list
- Teacher profile
- Search
- Edit
- Delete

---

## Class Management

- Classes
- Sections
- Student count
- Assigned teacher

---

## Subject Management

- Subjects
- Subject codes
- Assigned teachers

---

## Attendance

Students

- Present
- Absent
- Late

Teachers

- Present
- Absent
- Leave

Dashboard attendance summaries.

---

## Examination Management

- Exams
- Subjects
- Maximum marks

---

## Marks Management

- Student marks
- Edit
- Search
- Performance history

---

## AI Marksheet Upload

Upload:

- Image

AI extracts:

- Student name
- Roll number
- Class
- Section
- Subject
- Marks

---

## AI Review

Teacher can:

- Review
- Edit
- Delete
- Approve

before importing.

---

## Automatic Import

Automatically update:

- Student records
- Marks
- Dashboard
- Statistics

---

## AI Performance Summary

Generate insights including:

- Average marks
- Highest marks
- Lowest marks
- Students requiring attention

---

## Search

Global search across:

- Students
- Teachers
- Subjects
- Classes

---

## Settings

Basic school configuration.

---

# Features Excluded From MVP

Do not implement:

- Authentication
- Parent Portal
- Student Portal
- Fees Management
- Payment Gateway
- QR Attendance
- Face Recognition
- Biometric Attendance
- CCTV Integration
- Google Classroom
- Hostel Management
- Transport Management
- Payroll
- Library
- Inventory
- Multi-school Support

---

# Development Rules

Always:

- Build one feature at a time.
- Keep architecture clean.
- Reuse existing components.
- Avoid unnecessary dependencies.
- Preserve UI consistency.
- Write readable TypeScript.
- Minimize complexity.
- Verify changes before continuing.

Never:

- Rewrite completed modules.
- Refactor unrelated code.
- Add features outside the MVP.
- Break existing functionality.

---

# Definition of Done

A task is complete only when:

- The application builds successfully.
- No obvious runtime errors exist.
- Existing features continue working.
- UI remains consistent.
- Loading states exist.
- Empty states exist.
- Error handling exists.
- The feature can be demonstrated.

---

# Final Demo Flow

1. Open Dashboard.
2. View school statistics.
3. Browse Students.
4. Browse Teachers.
5. Upload a marksheet image.
6. AI extracts student records.
7. Review extracted data.
8. Approve import.
9. Database updates.
10. Dashboard refreshes.
11. Student marks update.
12. Display AI-generated performance summary.

This demonstration should clearly show how AI reduces manual administrative work in schools.

---

# Success Criteria

The project is considered successful if:

- The application is stable.
- The AI workflow works reliably.
- The interface looks professional.
- The demo can be completed smoothly.
- The codebase remains clean and maintainable.
- Judges can immediately understand the value of the product.
