Perfect format! Based on that, here's the **Markdown README** for **Day 2: User Authentication System** using Node.js, Express, MongoDB, bcrypt, and JWT:

---

# 🔐 User Authentication API - Node.js, Express, MongoDB, JWT

Welcome to Day 2 of my **10 Days of Node.js/Express/MongoDB** series!

This is a secure **User Authentication System** built with **Node.js**, **Express.js**, **MongoDB**, **bcrypt** for password hashing, and **JWT** for token-based authentication.

---

## 🚀 Features

- User Registration (Signup)
- User Login with JWT Token generation
- Password Hashing using bcrypt
- JWT-based Authentication
- Protected Route to fetch user data
- Organized folder structure
- Environment variables for sensitive config

---

## 🧠 Technologies Used

- Node.js  
- Express.js  
- MongoDB (local)  
- Mongoose  
- bcryptjs  
- jsonwebtoken  
- dotenv  

---

## 📁 Folder Structure

```
your-project/
├── models/
│   └── User.js
├── routes/
│   └── authRoutes.js
├── middleware/
│   └── authMiddleware.js
├── .env
├── index.js
├── package.json
└── README.md
```

---

## 📦 Installation & Setup

1. **Clone the repo**
```bash
git clone https://github.com/your-username/auth-api.git
cd auth-api
```

2. **Install dependencies**
```bash
npm install
```

3. **Create a `.env` file**
```
MONGO_URI=mongodb://127.0.0.1:27017/authdb
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

4. **Start the server**
```bash
npm run dev
```

Server will be running at:  
👉 `http://localhost:5000`

---

## 📬 API Endpoints

| Method | Endpoint         | Description              |
|--------|------------------|--------------------------|
| POST   | `/api/auth/register` | Register a new user    |
| POST   | `/api/auth/login`    | Login and get JWT token |
| GET    | `/api/auth/user`     | Get user info (Protected) |

---

## 🧪 Sample JSON for Register/Login

### ✅ Register

```json
{
  "name": "Yogesh",
  "email": "yogesh@example.com",
  "password": "password123"
}
```

### ✅ Login

```json
{
  "email": "yogesh@example.com",
  "password": "password123"
}
```

🔐 For accessing protected routes, send token in headers:
```
x-auth-token: your_jwt_token_here
```

---

## 🔥 Learning Goal

This project is part of my **#10Days10Projects** challenge to master backend development using Node.js, Express, and MongoDB.

I learned how to:
- Hash passwords securely with bcrypt
- Authenticate users using JWT
- Build middleware to protect routes

---

## 🧑‍💻 Author

**Yogesh Shinde**  
GitHub: [@y0geshshinde](https://github.com/y0geshshinde)  
LinkedIn: [@y0geshshinde](https://www.linkedin.com/in/y0geshshinde)

---

Let me know if you want a Markdown for Day 3 too when you're ready 🚀
