# Multi-Tenant SaaS Platform

This project is a fully dockerized **Multi-Tenant SaaS Platform** developed using **Node.js, PostgreSQL, React, and Docker**.  
It is designed to support **multiple tenants**, enforce **role-based access control**, and manage **projects and tasks** securely.

All services — database, backend API, and frontend UI — start together using a **single Docker Compose command**.

---

## Tech Stack

### Backend
- Node.js
- Express.js
- PostgreSQL
- JWT Authentication
- Role-Based Access Control (RBAC)

### Frontend
- React (Vite)
- Axios
- Role-based UI rendering

### Infrastructure
- Docker
- Docker Compose

---

## How to Run the Project (Mandatory)

### Prerequisites
Ensure the following are installed on your system:
- Docker
- Docker Compose

---

### ▶️ Start the Application

From the **project root directory**, run:

```bash
docker-compose up -d
````

This command will:

* Start the PostgreSQL database
* Execute database migrations and seed data
* Launch the backend API service
* Start the frontend application

⚠️ No manual database setup is required.

---

## Access the Application

| Service      | URL                                                                  |
| ------------ | -------------------------------------------------------------------- |
| Frontend     | [http://localhost:3000](http://localhost:3000)                       |
| Backend API  | [http://localhost:5000](http://localhost:5000)                       |
| Health Check | [http://localhost:5000/api/health](http://localhost:5000/api/health) |

---

## Authentication & Roles

The platform supports the following roles:

* **super_admin** – System-wide administrator
* **tenant_admin** – Tenant-level administrator
* **user** – Standard tenant user

Each tenant’s data is completely isolated from other tenants.

---

## Core Features

* Tenant registration and authentication
* Role-based user access control
* Project management
* Task management
* Secure JWT-based authentication
* Multi-tenant data isolation
* Fully containerized setup

---

## Testing the Application

After starting the application:

1. Open the frontend in a browser
2. Log in using credentials from `submission.json`
3. Verify:

   * Tenant isolation
   * Role-based access
   * Project and task functionality

---

## Demo Video

A demo video demonstrates:

* Application architecture
* Docker startup process
* Multi-tenant behavior
* User, project, and task workflows

👉Demo link https://drive.google.com/file/d/1eCa_ILdmBYGqQCw-YKaJYrYrkPZfcw7h/view?usp=sharing

---

## Notes for Evaluators

* The application is fully dockerized
* All services start with `docker-compose up -d`
* Database migrations and seed data load automatically
* No manual commands are required
* Repository is public and accessible
* Backend and frontend source code is included
* Database migration and seed files are provided
* The repository contains a minimum of 30 meaningful commits

````

