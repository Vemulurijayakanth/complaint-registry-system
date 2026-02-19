📘 Complaint Registry System (MERN Stack)

A full-stack Complaint Registry Web Application built using the MERN stack (MongoDB, Express.js, React, Node.js).
This project allows users to register complaints, track status, and communicate, while admins/agents manage and resolve complaints.

🚀 Features
👤 User Features

User registration & login with validation

Submit a new complaint

View complaint history

Track live complaint status

Chat window for interacting with support/agent

Simple and responsive UI

🛠️ Admin/Agent Features

Secure login

View all user complaints

Update complaint status (Pending → In Progress → Resolved)

Reply to user queries through chat

Dashboard for complaint management

🧩 Tech Stack
Frontend

React.js

React Router

Axios

CSS

Component-based folder structure

Backend

Node.js

Express.js

MongoDB (Mongoose ODM)

JSON Web Tokens (JWT)

bcrypt for password hashing

📦 Project Structure
complaint-registery/
│
├── backend/
│   ├── config/            # Database connection
│   ├── controllers/       # Business logic
│   ├── middleware/        # Auth middlewares
│   ├── models/            # MongoDB schemas
│   ├── routes/            # API routes
│   └── index.js           # Entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── user/          # User pages
│   │   ├── agent/         # Agent pages
│   │   ├── common/        # Shared pages (Login, Signup)
│   │   ├── Images/        # App images
│   │   └── index.js       # Frontend entry
│
└── README.md

🔧 Installation & Setup
1. Clone the repository
git clone https://github.com/yourusername/complaint-registery.git
cd complaint-registery

🖥️ Backend Setup (Node.js + Express)
2. Install backend dependencies
cd backend
npm install

3. Create Environment File

Create .env inside /backend:

MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_secret_key
PORT=5000

4. Start backend server
npm start


Backend runs on:
👉 http://localhost:5000

🎨 Frontend Setup (React)
5. Install frontend dependencies
cd ../frontend
npm install

6. Start frontend
npm start


Frontend runs on:
👉 http://localhost:3000

🔌 API Endpoints (Backend)
Auth
Method	Endpoint	Description
POST	/api/auth/register	Register new user
POST	/api/auth/login	Login user
User
Method	Endpoint	Description
POST	/api/complaint/add	Add complaint
GET	/api/complaint/list	Get user's complaints
Agent/Admin
Method	Endpoint	Description
GET	/api/admin/complaints	View all complaints
PUT	/api/admin/update/:id	Update status
📸 UI Preview

User Interface

Complaint Dashboard

Agent Panel

Chat Window

(Images available inside: frontend/src/Images/)

🛡️ Security Features

Hashed passwords using bcrypt

JWT-based secure authentication

Protected routes for users & agents

MongoDB safe schema validation

📚 Future Improvements

Email notifications

File upload for complaint proof

Admin analytics dashboard

Mobile app version

🤝 Contributing

Contributions are welcome!
Feel free to fork this repo & create a pull request