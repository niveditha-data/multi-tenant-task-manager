# Multi-Tenant Task Management System

# 🎯 My Approach: The "Safe-Share" Task System
*Internship Application - Center for Digital Infrastructure*

## 💡 The Problem I'm Solving
When multiple companies use the same software, the biggest risk is "Privacy Leaks." If Company A is using this system to manage secret projects, they should never even know that Company B exists on the same platform. 

## 🏗️ How I've Built the Logic
I approached this by thinking about a **Private Apartment Building**. Even though everyone shares the same roof (the software), every tenant has their own locked door.

### 1. The "Digital Lock" (Data Isolation)
In my design, every single task in the database is "stamped" with a **Tenant ID**. 
* **The Rule:** The system is programmed to only show data that matches the user's specific stamp. 
* **Example:** If I log in as a user from "Kerala Tech," the system automatically hides everything that doesn't have the "Kerala Tech" ID.

### 2. Who is in Charge? (Roles)
Inside each company, not everyone should see everything. I've designed two levels:
* **The Manager (Admin):** Can see the whole team's progress.
* **The Team Member (User):** Can only see the tasks they need to work on today. This keeps the workspace clean and secure.

## 🚀 Why I chose this design
I chose this specific design becouse, in my view,Security isnt an 'add-on' its the foundation. i wanted to focus on **Security First**. Before I write a single line of complex code, I want to ensure the architecture is safe for the users. I plan to build this using **Node.js** and **PostgreSQL** because they are industry standards for handling this kind of data isolation.

---
*“I believe great software isn't just about code, but about protecting the people who use it.”*

