# Architecture Rules

Keep the existing architecture.

Top-level folders:

- app
- components
- lib
- prisma
- public
- hooks
- styles
- types

Do not create additional top-level folders unless necessary.

Business logic should not exist inside UI components.

Database logic belongs in Prisma or server actions.

The AI module must not write directly to the database.

Teacher approval is required before importing AI-generated records.

Reuse components whenever possible.
