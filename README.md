# 📝 Task Manager App

A full-stack task management web application where users can register, log in, manage tasks, and securely upload and download related files. Admins can view all tasks from all users with their names. The app supports authentication, pagination, file uploads/downloads, and uses Docker for containerization.

---

## 🚀 Features

- 🔐 **Authentication** – Register and log in securely (JWT-based)
- 📝 **Task Management** – Add, edit, delete your own tasks
- 🗂 **File Upload/Download** – Upload files with your tasks and download them
- 📄 **Pagination** – Efficient task listing with page navigation
- 🧑‍💼 **Admin View** – Admin can view all users and their tasks
- 🐳 **Dockerized** – Easily run the project using Docker & Docker Compose

---

## 📦 Tech Stack

**Frontend:** React + Axios + Tailwind CSS  
**Backend:** Node.js + Express  
**Database:** MongoDB  
**Auth:** JWT (JSON Web Token)  
**File Uploads:** Multer  
**Containerization:** Docker & Docker Compose

---

## 🛠️ Installation Steps

### 🔧 Without Docker (For local development)

1. **Clone the repo:**

   ```bash
   git clone https://github.com/your-username/task-manager-app.git
   cd task-manager-app
   ```

2. **Setup Backend:**

   ```bash
   cd backend
   npm install
   npm run dev
   ```

3. **Setup Frontend:**

   Open a new terminal tab:

   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. Visit the app at:  
   ```
   http://localhost:5173/
   ```

---

### 🐳 With Docker (Recommended for testing and deployment)

1. **Run the full app with one command:**

   ```bash
   docker-compose up --build
   ```

2. Visit the app at:  
   ```
   http://localhost:5173/
   ```

---

## 🔐 Admin Credentials

> You can set admin credentials manually in the database or use the seed admin route if implemented.

Created by developer: 
Email: admin@example.com 
Password: Admin123
---

## 📁 API Documentation

**Base URL:** `http://localhost:5000/api`

| Method | Endpoint        | Description                    | Access        |
|--------|------------------|--------------------------------|---------------|
| POST   | `/auth/register` | Register a new user            | Public        |
| POST   | `/auth/login`    | Log in a user (returns token)  | Public        |
| GET    | `/tasks`         | Get user's tasks               | User/Private  |
| POST   | `/tasks`         | Create a new task              | User/Private  |
| PUT    | `/tasks/:id`     | Update a task                  | User/Private  |
| DELETE | `/tasks/:id`     | Delete a task                  | User/Private  |
| GET    | `/tasks/all`     | Admin: View all user tasks     | Admin Only    |
| GET    | `/files/:id`     | Download file by task ID       | User/Private  |

---

## 📷 Screenshots

(Attach screenshots of: Register/Login Page, Dashboard, Admin View, Pagination, File Upload)

---

## ✅ To Do (Optional Improvements)

- Add sorting/filtering by due date, status
- Add task priority levels
- Add email notifications
- Integrate CI/CD (GitHub Actions)

---

## 🧑‍💻 Author

**Anshika Pal**  
[GitHub](https://github.com/your-username)
