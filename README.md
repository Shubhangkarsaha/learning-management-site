# learning-management-site
📚 Learning Management System (LMS)

A full-stack medium-scale Learning Management System (LMS) built using the MERN stack.
This project provides a complete learning platform with authentication, course hosting, content access control, user activity tracking, orders, notifications, and an admin analytics dashboard.

🚀 Features
👤 User Features

Signup, login, logout

Account activation via email

Update profile, password, avatar

Token regeneration, secure sessions

Access purchased courses

Course content protection (valid users only)

Ask questions inside a course

Reply to questions

Add reviews to courses

Manage notifications

View orders and purchase history

📚 Course Features

Course model with lessons, videos, FAQs

Create/Edit courses (admin/instructor)

Get all courses without purchase

Get course content after purchase

Add questions & replies

Add reviews

Course analytics

🛒 Orders & Payments

Create orders

Track purchases

Order details stored in DB

🔔 Notification System

Notification model

Get all notifications

Update notification status

Auto-delete read notifications after a certain time

🛠️ Admin Features

Get all users, courses, orders

Add or remove members

Ban/unban users

Delete courses

Advanced analytics:

Last 28 days users

Orders

Notifications

1-year insights

🧠 Tech Stack
Frontend

React.js

React Router

Context API / Redux Toolkit

Axios

TailwindCSS / Material UI

Backend

Node.js

Express.js

MVC + Service Layer

Multer for uploads

Nodemailer for emails

Database

MongoDB

Mongoose

Cloud Storage

Cloudinary

Caching & Optimization

Redis

Security

JWT Authentication

Bcrypt Password Hashing

Rate Limiting

Validation Middlewares

🏛️ Architecture Diagram

📂 Folder Structure Diagram

📁 Folder Structure (Text View)
project/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   ├── config/
│   └── server.js
│
└── frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── context/
    │   ├── hooks/
    │   ├── utils/
    │   └── App.js
    └── package.json

⚙️ Installation & Setup
1. Clone the repository
git clone https://github.com/your-username/your-lms.git
cd your-lms

2. Install backend dependencies
cd backend
npm install

3. Install frontend dependencies
cd ../frontend
npm install

4. Create Environment Files
backend/.env
MONGO_URI=
JWT_SECRET=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
EMAIL_HOST=
EMAIL_USER=
EMAIL_PASS=
REDIS_URL=

frontend/.env
REACT_APP_API_URL=http://localhost:5000

▶️ Run the Project
Backend
cd backend
npm run dev

Frontend
cd frontend
npm start

🧪 API Overview (Short Summary)
Module	Endpoints
Auth	register, activate, login, logout, refresh token
User	get profile, update profile, avatar upload
Course	create, edit, list all, get single, content access
Q/A	create question, reply
Reviews	add review
Notifications	get, update, delete
Orders	create order, get user orders
Admin	users, courses, orders, analytics
