# Task Reminder and Tracking Application

A full-stack **Task Reminder and Tracking Application** built using **Spring Boot (Backend)** and **React + Vite (Frontend)**.

The application allows users to:
- Create and manage tasks
- Track task completion status
- Schedule reminders for tasks
- Export task reports as CSV
- View task overview statistics

This repository follows a **monorepo structure**, containing both backend and frontend in a single GitHub repository.

---

## Project Structure

Task-Reminder-and-Tracking-Application/  
├── task-reminder/ # Spring Boot Backend  
├── task-reminder-ui/ # React + Vite Frontend  
├── LICENSE # MIT License  
└── README.md # Root documentation (this file)

---

## 🧠 Application Overview

### 🔹 Backend (Spring Boot)
The backend is responsible for:
- Task creation, retrieval, and updates
- Task completion tracking
- Scheduling task reminders
- Generating CSV reports
- Providing task overview statistics

**Key features:**
- RESTful APIs
- JDBC with `JdbcTemplate`
- H2 in-memory database
- ScheduledExecutorService for reminders
- Mock email notification system
- Centralized exception handling
- Swagger (OpenAPI) documentation

📄 Detailed backend documentation is available at:  
task-reminder/README.md

---

### 🔹 Frontend (React + Vite)
The frontend provides a simple dashboard to:
- View all tasks
- Add new tasks with due date & time
- Mark tasks as completed
- Schedule reminders from UI
- View task status (Pending / Completed)

The frontend communicates with the backend using REST APIs.

📄 Detailed frontend documentation is available at:  
task-reminder-ui/README.md

---

## 🛠️ Tech Stack

### Backend
- Java 21
- Spring Boot
- JDBC (JdbcTemplate)
- H2 In-Memory Database
- Maven
- Swagger (OpenAPI)

### Frontend
- React
- Vite
- JavaScript
- HTML / CSS
- Fetch API

---

## 📘 API Documentation (Swagger)

Swagger UI is integrated to provide interactive and user-friendly API documentation.

### 🔗 Access Swagger UI
Once the backend application is running, open the following URL in your browser:

http://localhost:8081/swagger-ui/index.html

### 🚀 Features
- Interactive API exploration
- Clear request and response schemas
- Easy API testing directly from the browser (no Postman required)

---

## 🔗 Frontend ↔ Backend API Mapping

| Feature               | API Endpoint                   |
|----------------------|--------------------------------|
| Fetch all tasks       | `GET /tasks`                   |
| Add task              | `POST /tasks`                  |
| Mark task completed   | `PUT /completion/mark/{id}`    |
| Schedule reminder     | `POST /schedule/set`           |
| Get reminder status   | `GET /schedule/reminders/{id}` |
| Get task status       | `GET /completion/status/{id}`  |
| Export CSV report     | `POST /reports/export`         |
| Task overview summary | `GET /reports/overview`        |

---

## ▶️ How to Run the Project Locally

### 1️⃣ Run Backend

```bash
cd task-reminder
mvn spring-boot:run
Backend will start at:

http://localhost:8081

H2 Database Console:

http://localhost:8081/h2-console

2️⃣ Run Frontend
bash
Copy code
cd task-reminder-ui
npm install
npm run dev
Frontend will start at:

http://localhost:5173

🧪 Testing
All backend APIs tested using Postman & Swagger UI

Reminder lifecycle verified

CSV export validated

Frontend tested manually through browser

Backend and frontend integration verified

Full-stack application development

REST API design

Frontend–backend integration

Scheduling and concurrency concepts

Clean architecture and code organization

Proper version control using Git and GitHub

📜 License
This project is licensed under the MIT License.

You are free to:

Use

Modify

Distribute

Publish



