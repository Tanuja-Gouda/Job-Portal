# 📝 Job Portal — MERN Stack Project

A full-featured Job Portal web application built with the **MERN stack** (MongoDB, Express, React, Node.js).  
It allows users to register, log in, view job listings, apply for jobs, and enables recruiters to post and manage job vacancies.

---

## 📌 Features

- 👥 User Registration and Login with JWT Authentication
- 📄 Recruiters can post, update, and delete job listings
- 📝 Job seekers can view available jobs and apply
- 🔐 Passwords securely hashed using bcrypt
- 📦 RESTful API-based backend with Express.js
- 💾 MongoDB for storing users, jobs, and application data
- ⚛️ React frontend with modern UI and routing
- 📡 Axios used for frontend-backend API communication

---

## 🖥️ Tech Stack

| Technology | Description                        |
|------------|------------------------------------|
| React.js   | Frontend library for UI development|
| Node.js    | Backend runtime environment        |
| Express.js | Web framework for Node.js          |
| MongoDB    | NoSQL database                     |
| Mongoose   | MongoDB ORM for Node.js            |
| Axios      | HTTP client for API requests       |
| JWT        | Secure token-based authentication  |
| Bcrypt     | Password hashing                   |

---

## 📂 Project Structure

```
jobportal-yt/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   ├── .env
│   ├── server.js
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   ├── index.js
│   ├── package.json
├── package.json
├── README.md
```

---

## ⚙️ Installation & Setup

### 📌 Prerequisites
- Node.js & npm
- MongoDB (local or cloud-based like MongoDB Atlas)

---

### 📦 Backend Setup

```bash
cd backend
npm install
```

- Create a `.env` file in `backend/` with the following:
  ```
  MONGO_URI=your_mongo_connection_string
  JWT_SECRET=your_jwt_secret_key
  PORT=5000
  ```

- Run the backend server:
  ```bash
  npm start
  ```

---

### ⚛️ Frontend Setup

```bash
cd frontend
npm install
```

- Start the React development server:
  ```bash
  npm start
  ```

---

## 🔗 API Endpoints Overview

| Method | Endpoint              | Description                    |
|:--------|:---------------------|:--------------------------------|
| POST   | `/auth/register`      | Register a new user             |
| POST   | `/auth/login`         | User login and get JWT          |
| GET    | `/jobs`               | Fetch all job listings          |
| POST   | `/jobs`               | Add a new job (Recruiter only)  |
| DELETE | `/jobs/:id`           | Delete a job (Recruiter only)   |
| POST   | `/jobs/:id/apply`     | Apply to a job (User only)      |

---

## 🔐 Authentication & Security

- Passwords are hashed using `bcrypt`
- JWT tokens issued on login for secure authentication
- Protected routes implemented with middleware

---

## 🚀 Future Enhancements

- Integrate real-time notifications for job application status
- Implement email verification and password reset functionality
- Add AI-powered resume screening and suggestions based on company/job requirements

