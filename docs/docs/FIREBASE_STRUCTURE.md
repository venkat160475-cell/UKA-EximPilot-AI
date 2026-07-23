# UKA EximPilot AI

# FIREBASE STRUCTURE

Version: 1.0

---

# Technology Stack

Frontend
- React

Backend
- Firebase

Database
- Cloud Firestore

Authentication
- Firebase Authentication

Storage
- Firebase Storage

Hosting
- Firebase Hosting

Version Control
- GitHub

AI
- Google AI Studio (Gemini)

---

# Firebase Services

## Authentication

Supported Login Methods

- Email & Password
- Google Sign-In (Future)

User Roles

- Super Admin
- Admin
- Sales Manager
- Sales Executive
- Marketing Executive
- Documentation Executive
- Finance
- Accounts
- Viewer

---

# Cloud Firestore

Collections

users
organizations
companies
contacts
prospects
leads
meetings
followups
tasks
government_services
rodtep_claims
documents
quotations
agreements
invoices
payments
reports
notifications
knowledge_base
email_templates
whatsapp_templates
ai_insights
audit_logs
settings
backup_history

---

# Firebase Storage

Folder Structure

/company-documents/

/company-documents/{companyId}/IEC/

/company-documents/{companyId}/GST/

/company-documents/{companyId}/PAN/

/company-documents/{companyId}/ShippingBills/

/company-documents/{companyId}/Invoices/

/company-documents/{companyId}/PackingList/

/company-documents/{companyId}/BillOfLading/

/company-documents/{companyId}/eBRC/

/company-documents/{companyId}/Certificates/

/company-documents/{companyId}/Emails/

/company-documents/{companyId}/Other/

---

# AI Processed Documents

/ai/

/ocr/

/summaries/

/recommendations/

---

# User Profile Images

/users/profile-images/

---

# Company Logos

/company-logos/

---

# Security Rules

Users can access only data they are permitted to see.

Super Admin

- Full Access

Admin

- Organization Access

Sales

- Assigned Customers
- Assigned Leads

Finance

- Billing
- Payments

Documentation Team

- Documents
- Claims

---

# Environment Variables

VITE_FIREBASE_API_KEY

VITE_FIREBASE_AUTH_DOMAIN

VITE_FIREBASE_PROJECT_ID

VITE_FIREBASE_STORAGE_BUCKET

VITE_FIREBASE_MESSAGING_SENDER_ID

VITE_FIREBASE_APP_ID

---

# Hosting

Firebase Hosting

Future

Custom Domain

SSL

Automatic Deployment

---

# Multi Organization Support

Organization

↓

Users

↓

Companies

↓

Contacts

↓

Business Modules

Each organization's data remains isolated.

---

# Backup Strategy

Super Admin Only

Backup Firestore

Export Excel

Restore Data

Download Reports

---

# Audit Logs

Track

User

Date

Module

Action

IP Address (Future)

Device (Future)

---

# Notification Engine

Email

WhatsApp

Dashboard Alerts

Push Notifications (Future)

---

# Future Integrations

DGFT

ICEGATE

GST

PAN Verification

Email

WhatsApp

LinkedIn

Google Maps

IndiaMART

TradeIndia

ExportersIndia

---

# Deployment Workflow

GitHub

↓

Google AI Studio

↓

Firebase

↓

Production

---

# Version

1.0
