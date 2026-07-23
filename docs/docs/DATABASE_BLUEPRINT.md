# UKA EximPilot AI

# DATABASE BLUEPRINT

Version: 1.0

---

# Database

Google Cloud Firestore

---

# Collections

## users

Stores all application users.

Fields

- userId
- name
- email
- mobile
- role
- organizationId
- status
- lastLogin
- createdAt

---

## organizations

Supports future multi-organization architecture.

Fields

- organizationName
- companyLogo
- subscription
- status
- createdAt

---

## companies

Stores Company Master.

Fields

- companyName
- legalName
- tradeName
- industry
- businessStatus
- companyType
- iecNumber
- gstNumber
- pan
- cin
- msme
- lut
- rcmc
- icegate
- adCode
- exportProducts
- importProducts
- exportCountries
- importCountries
- annualTurnover
- exportTurnover
- manufacturingAddress
- factoryAddress
- billingAddress
- website
- linkedIn
- customerSince
- assignedExecutive
- createdAt
- updatedAt

---

## contacts

Unlimited contacts per company.

Fields

- companyId
- fullName
- designation
- department
- mobile
- alternateMobile
- whatsapp
- email
- linkedIn
- birthday
- decisionMaker
- preferredLanguage
- preferredContactMethod
- bestTimeToCall
- relationshipScore
- status

---

## prospects

Future B2B Directory.

Fields

- companyName
- industry
- city
- state
- source
- website
- linkedIn
- status
- notes

---

## leads

Fields

- leadNumber
- companyId
- contactId
- leadSource
- assignedTo
- stage
- leadScore
- businessPotentialScore
- expectedRevenue
- expectedConsultancyFee
- nextFollowUp
- aiRecommendation
- createdAt

---

## meetings

Fields

- meetingDate
- companyId
- contactId
- discussion
- actionItems
- nextMeeting
- aiSummary

---

## followups

Fields

- followUpDate
- companyId
- contactId
- followUpType
- notes
- result
- nextFollowUp
- priority

---

## tasks

Fields

- taskTitle
- assignedTo
- companyId
- dueDate
- priority
- status
- reminder

---

## government_services

Fields

- companyId
- serviceType
- applicationNumber
- status
- remarks

---

## rodtep_claims

Fields

- shippingBillNumber
- shippingDate
- port
- invoiceNumber
- hsCode
- fobValue
- schemeRate
- benefitAmount
- claimStatus
- approvalDate
- paymentDate
- errorStatus

---

## documents

Fields

- companyId
- documentType
- fileName
- storagePath
- uploadedBy
- uploadedDate
- expiryDate
- aiExtractedData

---

## quotations

Fields

- quotationNumber
- companyId
- amount
- gst
- status

---

## invoices

Fields

- invoiceNumber
- companyId
- invoiceDate
- amount
- gst
- paymentStatus

---

## payments

Fields

- paymentDate
- amount
- paymentMode
- referenceNumber

---

## notifications

Fields

- title
- description
- type
- priority
- status

---

## ai_insights

Fields

- companyId
- customerHealth
- churnRisk
- upsellOpportunity
- nextBestAction
- aiSummary

---

## audit_logs

Fields

- user
- action
- module
- timestamp

---

## knowledge_base

Fields

- category
- title
- document
- keywords
- source

---

## reports

Stores generated reports.

---

## settings

Stores system configuration.

---

## email_templates

Stores reusable email templates.

---

## whatsapp_templates

Stores WhatsApp templates.

---

## backup_history

Tracks backups created by Super Admin.

---

# Relationships

Organization
    ↓
Companies
    ↓
Contacts
    ↓
Leads
    ↓
Meetings
    ↓
Follow-ups
    ↓
Tasks
    ↓
Proposals
    ↓
Invoices
    ↓
Payments

All modules connect back to Company Master.
