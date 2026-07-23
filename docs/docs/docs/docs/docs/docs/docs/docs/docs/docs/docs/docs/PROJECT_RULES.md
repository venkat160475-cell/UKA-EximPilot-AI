# UKA EximPilot AI

# PROJECT RULES

Version: 1.0

---

# Purpose

This document defines the permanent development rules for UKA EximPilot AI.

Every future module must follow these rules.

---

# Rule 1 - Never Break Existing Modules

New modules must never modify or break completed modules unless intentionally upgrading them.

---

# Rule 2 - Build Reusable Components

Every page should reuse components wherever possible.

Examples

- Tables
- Cards
- Forms
- Buttons
- Search Bars
- Filters
- Status Badges
- Dialog Boxes

---

# Rule 3 - Mobile Responsive

Every screen must work on:

- Desktop
- Laptop
- Tablet
- Mobile

---

# Rule 4 - AI First

Every module should include AI where it adds value.

Examples

- AI Suggestions
- AI Alerts
- AI Recommendations
- AI Summaries
- AI Predictions

---

# Rule 5 - Company-Centric Design

Every business record should relate to a Company.

Company

↓

Contacts

↓

Leads

↓

Meetings

↓

Tasks

↓

Government Services

↓

RoDTEP Claims

↓

Documents

↓

Invoices

↓

Payments

---

# Rule 6 - Prospect First

Prospects are potential future customers.

Prospects should be convertible into Leads.

Leads should be convertible into Customers.

---

# Rule 7 - Data Security

Only authorized users can access data.

Role-based permissions must be enforced.

---

# Rule 8 - Super Admin

Only Super Admin can:

- Import Excel
- Export Excel
- Backup Database
- Restore Database
- Manage Users
- Manage Roles
- View Audit Logs
- Configure System Settings

---

# Rule 9 - No Hardcoded Business Data

Business records must come from Firestore.

Configuration belongs in configuration files.

Secrets belong in environment variables.

---

# Rule 10 - AI Never Makes Final Decisions

AI may:

- Suggest
- Recommend
- Summarize
- Predict

AI must not approve, reject, or alter important business records without user confirmation.

---

# Rule 11 - Consistent User Interface

Every module should follow:

- UI_GUIDELINES.md
- BUSINESS_RULES.md
- FIREBASE_STRUCTURE.md

---

# Rule 12 - Documentation

Every completed module must update:

- MODULE_STATUS.md
- CHANGELOG.md

Major architecture changes should also update:

- MASTER_PLAN.md
- DATABASE_BLUEPRINT.md

---

# Rule 13 - Coding Standards

- Keep components small.
- Use descriptive names.
- Avoid duplicate logic.
- Organize folders consistently.
- Prefer reusable code.

---

# Rule 14 - AI Context

Before building a new module, review:

- MASTER_PLAN.md
- MODULE_STATUS.md
- BUSINESS_RULES.md
- UI_GUIDELINES.md
- DATABASE_BLUEPRINT.md

This ensures consistency across the project.

---

# Rule 15 - Version Strategy

Version 1

Focus on delivering a stable AI-powered CRM for:

- Marketing
- Sales
- Import & Export Consultancy
- Government Schemes
- RoDTEP
- Billing
- AI Assistant

Version 2

Add:

- B2B Directory
- Mobile App
- Voice AI
- Advanced Analytics
- Enterprise Features

---

# Project Principle

Every feature should answer one question:

"Does this help UKA Exim Enterprises serve customers faster, better, and more intelligently?"

If the answer is yes, it belongs in UKA EximPilot AI.
