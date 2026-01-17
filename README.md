# AppSec Notes Lab

This repository is a long-term learning project focused on:
- building real web applications,
- understanding how they fail,
- learning Application Security and Bug Bounty in a practical way.

This is NOT a tutorial project.
This is a growing lab that evolves from a simple application into a security-focused system.

---

## Final Goal

Build a realistic web application and iteratively:
- design features,
- implement backend logic,
- introduce security vulnerabilities intentionally,
- exploit them,
- fix them,
- document findings like real AppSec / Bug Bounty reports.

The goal is to understand **how vulnerabilities emerge from application logic**, not just how to exploit them.

---

## Architecture Overview

The project will consist of the following parts:

### 1. Backend API (Core of the project)
- Node.js + Express
- REST API design
- Request / Response lifecycle
- Business logic implementation
- Authentication and authorization
- Data validation
- Error handling

This is where most security bugs live.

---

### 2. Database Layer
- SQLite (initially)
- SQL basics
- Relations between entities
- Ownership of resources
- Query safety
- Logical data access control

Focus:
- IDOR
- Broken access control
- Data exposure

---

### 3. Authentication & Authorization
- User registration and login
- Password hashing
- JWT-based authentication
- Role-based access control (RBAC)
- Permission checks

Focus:
- Auth bypass
- Token misuse
- Trust boundary mistakes

---

### 4. Frontend (Minimal, Functional)
- HTML
- Vanilla JavaScript
- Fetch API
- Handling authentication tokens
- Understanding what the browser sends to the backend

Frontend is treated as an **attack surface**, not a security layer.

---

### 5. Security Vulnerabilities (Intentional)
The application will intentionally include vulnerabilities such as:
- IDOR (Insecure Direct Object Reference)
- Broken Access Control
- Authentication flaws
- Business logic vulnerabilities
- Missing validation
- Race conditions (later stages)
- Insecure file handling (later stages)

Each vulnerability will be:
- introduced intentionally,
- exploited manually,
- fixed properly,
- documented.

---

### 6. Vulnerability Documentation
Each security issue will be documented in `/docs`:
- vulnerability description
- reproduction steps
- impact analysis
- root cause
- fix explanation

This mimics:
- real AppSec work,
- real Bug Bounty reports.

---

## Learning Roadmap (What this project teaches)

### Web & Backend Fundamentals
- HTTP / HTTPS
- REST APIs
- Request lifecycle
- JSON handling
- Middleware logic

### Programming (Focused, Practical)
- Reading backend code
- Writing simple backend logic
- Understanding data flow
- Modifying existing code safely

### Application Security
- OWASP Top 10 (in practice, not theory)
- Secure coding principles
- Threat modeling
- Risk-based thinking

### Bug Bounty Skills
- Manual testing
- Logic flaw discovery
- API abuse
- Authorization testing
- Report writing

---

## Project Evolution Plan

### Phase 1 – Core Application
- Basic backend API
- User system
- Notes CRUD
- Simple frontend

### Phase 2 – Security Foundations
- Authentication & authorization
- Ownership checks
- Input validation
- First intentional vulnerabilities

### Phase 3 – Advanced Logic
- Sharing features
- Role separation
- Workflow logic
- Business logic flaws

### Phase 4 – Advanced Security Topics
- Rate limiting
- File uploads
- Token lifecycle
- Audit logging
- API abuse scenarios

---

## What This Project Is NOT
- Not a frontend showcase
- Not a framework comparison
- Not a CTF challenge
- Not a quick tutorial

This project is meant to grow with my skills and reflect real-world application security work.

---

## Status
🚧 In progress – foundation phase
