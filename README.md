# Multi-Tenant Task Management System

## 🚀 Project Concept
This is a conceptual design for a scalable task management system that supports multiple organizations (tenants) on a single platform while ensuring high security and data isolation.

## 🛠️ Key Architectural Pillars

### 1. Multi-Tenancy & Data Isolation
To ensure that "Organization A" can never see "Organization B's" tasks, I have designed the system using **Logical Isolation**. 
* Every table in the database will include a `tenant_id`.
* When a user logs in, the system identifies their `tenant_id` and automatically filters all database queries.

### 2. Role-Based Access Control (RBAC)
The system manages permissions through specific roles:
* **Admin:** Can create, edit, and delete all tasks within their own organization.
* **User:** Can only view and manage tasks specifically assigned to them.

## 📈 Planned Tech Stack
As I progress in my learning journey, I plan to build this using:
* **Frontend:** React.js (for a responsive user interface).
* **Backend:** Node.js with Express (to handle API logic).
* **Database:** PostgreSQL (to manage relational data and tenant isolation).

---
*Developed by Niveditha as part of the Centre for Digital Infrastructure Internship Application.*
