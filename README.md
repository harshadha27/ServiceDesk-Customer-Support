# ServiceDesk-Customer-Support
AI-powered customer support ticket management system with CRM-style workflows, ticket assignment, SLA tracking, dashboards, reports, and Gemini AI assistance.
# ServiceDesk – Customer Support Ticket Management System

ServiceDesk is a modern customer support ticket management system designed
to centralize customer support operations.

The application allows support teams to manage customers, support agents,
tickets, priorities, assignments, ticket statuses, SLA information,
comments, reports, and dashboards from a single platform.

It also includes an optional AI-powered Ticket Assistant using the Gemini API
to help summarize tickets, suggest categories and priorities, and generate
professional response suggestions.

---

## 🚀 Project Overview

Customer support teams need to manage a large number of customer requests,
assign tickets to support agents, prioritize urgent issues, track resolution
progress, and monitor team performance.

ServiceDesk provides a centralized CRM-style solution for managing this
workflow.

### Main Workflow

Customer
↓
Support Ticket
↓
Assignment
↓
Support Agent
↓
Investigation
↓
Resolution
↓
Closed

---

## 🎯 Objectives

- Centralize customer support information
- Manage customer records
- Manage support agents
- Create and track support tickets
- Assign tickets to support agents
- Manage ticket priorities
- Track ticket status
- Monitor SLA and due dates
- Maintain ticket history
- Generate support reports
- Visualize support metrics through dashboards
- Provide AI-assisted ticket analysis

---

## 🛠️ Technologies

### Frontend

- React
- TypeScript
- Vite
- HTML5
- CSS

### Database & Backend Services

- Firebase
- Cloud Firestore
- Firebase Authentication

### AI

- Google Gemini API
- Generative AI

### Development Tools

- Git
- GitHub
- VS Code
- Google AI Studio

---

## ✨ Features

### 👥 Customer Management

- Create customers
- Edit customers
- Delete customers
- Search customers
- View customer details
- View customer ticket history

### 👨‍💻 Support Agent Management

- Manage support agents
- Track agent availability
- Track assigned tickets
- View agent workload
- Monitor resolved tickets

### 🎫 Ticket Management

- Create support tickets
- Assign tickets
- Set ticket priority
- Set ticket category
- Update ticket status
- Add resolution notes
- Add comments
- Track ticket history

### ⚡ Ticket Automation

The system supports automated ticket workflows including:

- Initial ticket status
- Agent assignment
- Priority-based SLA calculation
- Due date calculation
- Resolution date tracking
- Ticket status transitions

### ⏱️ SLA Tracking

Tickets can be assigned SLA targets based on priority.

Example:

| Priority | SLA |
|---|---|
| Critical | 4 hours |
| High | 8 hours |
| Medium | 24 hours |
| Low | 48 hours |

The application can identify tickets as:

- On Track
- Due Soon
- Overdue
- Resolved

### 📊 Dashboard

The dashboard provides:

- Total Tickets
- Open Tickets
- In Progress Tickets
- Resolved Tickets
- Closed Tickets
- Critical Tickets
- Overdue Tickets
- Available Agents

### 📈 Reports

The application provides reports for:

- Open Tickets
- Critical Tickets
- Overdue Tickets
- Tickets by Agent
- Tickets by Category
- Resolved Tickets
- Closed Tickets
- Customer-wise Tickets
- Agent Workload
- Resolution Performance

### 🤖 AI Ticket Assistant

The optional Gemini-powered assistant can help with:

- Ticket summarization
- Category suggestions
- Priority suggestions
- Customer issue identification
- Professional response suggestions

AI-generated results are presented as suggestions and should be reviewed
by support personnel before being used.

---

## 🗂️ Main Data Entities

### Customer

Stores customer information.

Example fields:

- Customer ID
- Full Name
- Email
- Phone
- Company
- Industry
- Location
- Customer Status
- Created Date

### Support Agent

Stores support team information.

Example fields:

- Agent ID
- Full Name
- Email
- Department
- Role
- Availability
- Skills
- Active Tickets

### Ticket

Stores customer support requests.

Example fields:

- Ticket ID
- Subject
- Description
- Customer
- Assigned Agent
- Category
- Priority
- Status
- Created Date
- Updated Date
- Due Date
- Resolution Date
- Resolution Notes

### Comments

Stores ticket conversations and internal notes.

---

## 🔗 Relationships

The main relationships are:

Customer
↓
Tickets

Agent
↓
Assigned Tickets

Category
↓
Tickets

Each ticket is associated with:

- One customer
- One assigned agent
- One category

---

## 🔄 Ticket Lifecycle

```text
New
 ↓
Open
 ↓
In Progress
 ↓
Waiting for Customer
 ↓
Resolved
 ↓
Closed
