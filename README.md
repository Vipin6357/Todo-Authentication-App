🚀 MERN Todo App with Authentication

A complete full-stack Todo application built using the MERN stack, featuring secure JWT authentication and a modern UI.

🛠 Tech Stack
MongoDB — NoSQL database for storing users & todos
Express.js — Backend framework for APIs
React.js (Vite + Tailwind CSS) — Frontend UI
Node.js — Server runtime environment
✨ Key Features
🔐 Secure user authentication using JWT
🔑 Password encryption with bcrypt
🛡 Protected routes on both frontend & backend
📝 Complete CRUD operations for todos
🎯 Set priority levels (Low / Medium / High)
✅ Toggle task completion status
🔍 Filter tasks by priority and status
🔎 Search functionality for todos
🧹 Option to clear all completed tasks
💪 Password strength indicator
🎨 Stylish glassmorphism dark UI
📱 Fully responsive design
🔔 Toast notifications for actions



📁 Project Structure

mern-todo/
├── backend/
│   ├── controllers/
│   │   ├── authController.js
│   │   └── todoController.js
│   ├── middleware/
│   │   └── authMiddleware.js
│   ├── models/
│   │   ├── User.js
│   │   └── Todo.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   └── todoRoutes.js
│   ├── .env.example
│   ├── package.json
│   └── server.js
└── frontend/
    ├── src/
    │   ├── api/
    │   │   └── axios.js
    │   ├── components/
    │   │   ├── StatsBar.jsx
    │   │   ├── TodoForm.jsx
    │   │   └── TodoItem.jsx
    │   ├── context/
    │   │   └── AuthContext.jsx
    │   ├── pages/
    │   │   ├── Dashboard.jsx
    │   │   ├── Login.jsx
    │   │   └── Register.jsx
    │   ├── App.jsx
    │   ├── index.css
    │   └── main.jsx
    ├── index.html
    ├── package.json
    ├── tailwind.config.js
    └── vite.config.js




🔗 API Endpoints

| Method | Endpoint                | Access  | Description             |
| ------ | ----------------------- | ------- | ----------------------- |
| POST   | `/api/auth/register`    | Public  | Create a new user       |
| POST   | `/api/auth/login`       | Public  | Authenticate user       |
| GET    | `/api/auth/me`          | Private | Get logged-in user info |
| GET    | `/api/todos`            | Private | Retrieve all todos      |
| POST   | `/api/todos`            | Private | Add a new todo          |
| PUT    | `/api/todos/:id`        | Private | Update existing todo    |
| DELETE | `/api/todos/:id`        | Private | Remove a todo           |
| PATCH  | `/api/todos/:id/toggle` | Private | Toggle completion       |





⚙️ Installation & Setup
📌 Requirements
Node.js (v18 or higher)
MongoDB (Local instance or Atlas)



🔹 Backend Setup

cd backend
cp .env.example .env

Update your .env file:

PORT=5000
MONGO_URI=mongodb://localhost:27017/mern-todo
JWT_SECRET=your_secret_key_here
JWT_EXPIRE=7d


Run backend:

npm install
npm run dev

Server will start at:
👉 http://localhost:5000


🔹 Frontend Setup

cd frontend
npm install
npm run dev

Frontend will run at:
👉 http://localhost:5173

🌐 Access the App

Open your browser and go to:

👉 http://localhost:5173

Register a new account and start managing your tasks 🚀



☁️ MongoDB Atlas Setup (Optional)
Visit: https://www.mongodb.com/atlas
Create a free cluster
Copy your connection string
Replace MONGO_URI in .env:

MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/mern-todo


❤️ Credits

Developed with dedication using the MERN stack.

👉 This project is created by Vipin Gangwar 💻✨

