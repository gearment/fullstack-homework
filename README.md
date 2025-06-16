# Gearment Fullstack Homework

A take-home assignment for evaluating fullstack engineers with a focus on relational database design, REST API development, and responsive UI implementation using **ReactJS**.

---

## 📘 Objective

Design and implement a simple **Leave Management System** where employees can request leave and managers can approve/reject them.

---

## 🧠 Requirements

### 1. Relational Database (PostgreSQL or MySQL)

Design a normalized schema with at least the following tables:

- `users`: name, email, role (employee, manager)
- `leave_requests`: start_date, end_date, reason, status, created_by, approved_by
- `leave_balances`: user_id, year, total_days, used_days

> Bonus: Add support for leave types (e.g., sick leave, unpaid leave)

---

### 2. Backend API

You may use any backend framework (e.g., Node.js/Express, Go, Django).

Required endpoints:

| Endpoint                     | Method | Auth | Description                          |
|-----------------------------|--------|------|--------------------------------------|
| `/api/login`                | POST   | ❌    | Simulate login (hardcoded or mocked) |
| `/api/leave-request`        | POST   | ✅    | Create a leave request               |
| `/api/leave-request`        | GET    | ✅    | View your leave requests             |
| `/api/leave-request/all`    | GET    | ✅    | Manager: View team leave requests    |
| `/api/leave-request/:id`    | PATCH  | ✅    | Approve or reject a request          |
| `/api/leave-balance`        | GET    | ✅    | View current leave balance           |

> ✅ Use JWT or a simple session-based mock login system

---

### 3. Frontend (ReactJS)

Use React (via CRA or Vite) to build the UI.

#### Employee View:
- Login screen
- Dashboard showing leave balance and past requests
- Form to submit new leave requests

#### Manager View:
- View pending leave requests
- Approve or reject each request (modal or inline)

> UI must be responsive and work on both desktop and mobile

---

## 📦 Folder Structure

```sh
fullstack-homework/
├── frontend/           # React + Bootstrap
├── backend/            # REST API
├── database/           # SQL schema / migrations
├── README.md           # This file
└── docker-compose.yml  # (Optional for fullstack setup)
```

---

## ⚙️ Bonus Points

- Dockerized setup (`docker-compose`)
- Table filtering/search for manager view
- Unit tests for backend APIs
- Clear API response formats and error handling

---

## 🕐 Estimated Time

Working days: 7 days, bonus points come with the earlier submission

---

## ✅ Submission Guidelines

1. Fork this repository or upload to your GitHub
2. Include setup steps in a `README.md` inside each folder (`frontend/`, `backend/`)
3. Optionally deploy or record a demo video
4. Submit the repo link for review

---

## 📮 Questions?

If you have any questions or need clarifications, feel free to reach out to the hiring team at tech@gearment.com.

Good luck and have fun!
