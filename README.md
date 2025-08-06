# 📝 Task Manager App for PanScience Innovations

## Deployed URL: 
https://psi-assignment-client.vercel.app

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
   git clone https://github.com/your-username/PSI-Assignment.git
   cd PSI-Assignment
   ```

2. **Setup Backend:**

   ```bash
   cd backend
   npm install
   npm start
   ```

3. **Setup Frontend:**

   Open a new terminal tab:

   ```bash
   cd frontend
   npm install
   npm start
   ```

4. Visit the app at:  
   ```
   http://localhost:3000/
   ```

---

### 🐳 With Docker (Recommended for testing and deployment)

1. **Run the full app with one command:**

   ```bash
   docker-compose up --build
   ```

2. Visit the app at:  
   ```
   http://localhost:3000/
   ```

---

## 🔐 Admin Credentials

> You can set admin credentials manually in the database or use the seed admin route if implemented.

#### Created by developer: 
#### Email: admin@example.com 
#### Password: Admin123
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
### Home Page
<img width="1869" height="910" alt="image" src="https://github.com/user-attachments/assets/fd116812-042d-4d84-a429-b0c78819c064" />

### Register
<img width="1667" height="830" alt="image" src="https://github.com/user-attachments/assets/101b683d-b1e9-4f8f-96e9-88eb29cf48b0" />

### Login
<img width="1563" height="726" alt="image" src="https://github.com/user-attachments/assets/a9e31214-6d59-41c9-b67a-6c88733c55cb" />

 ### Admin Panel
 <img width="1899" height="913" alt="image" src="https://github.com/user-attachments/assets/b4993b50-4b73-4800-ac7c-2ed90f942df0" />
<img width="1387" height="864" alt="image" src="https://github.com/user-attachments/assets/158f0182-d5cb-46ac-a73f-9d6802e8c1fe" />

### User Panel
<img width="1876" height="901" alt="image" src="https://github.com/user-attachments/assets/df48a90d-7825-4a0e-85b1-c3447705ebf5" />
<img width="1802" height="913" alt="image" src="https://github.com/user-attachments/assets/3bc3c8e4-a1ea-41e3-8f80-11f6a9a0fe95" />



---

## 🧑‍💻 Author

**Anshika Pal**  
[GitHub](https://github.com/your-username)
