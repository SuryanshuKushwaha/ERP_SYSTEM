# ERP_SYSTEM

A full-stack **ERP (Enterprise Resource Planning) System** designed to digitize and automate organizational workflows such as HR management, employee services, and administrative operations.

---

## 📌 Project Overview

The ERP System simplifies internal business processes by providing role-based access for **Admins** and **Employees**, enabling efficient management of leaves, salary slips, enquiries, and quotations through a secure and scalable web application.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- JWT-based authentication
- Role-Based Access Control (RBAC)
- Secure login for Admins and Employees

### 👨‍💼 Admin Panel
- Manage employees
- Approve/reject leave requests
- Generate and upload salary slips (PDF)
- Handle enquiries and quotations

### 👩‍💻 Employee Panel
- Apply for leave
- View leave status
- Download salary slips
- Submit enquiries

### 📄 File & PDF Handling
- Salary slip generation
- Secure PDF upload and download

---

## 🛠 Tech Stack

### Frontend
- React.js
- HTML, CSS, JavaScript

### Backend
- Node.js
- Express.js

### Database
- MongoDB

### Other Tools & Libraries
- JWT (Authentication)
- Multer (File Upload)
- pdf-lib (PDF handling)
- REST APIs

---

## 📁 Folder Structure (Simplified)

ERP_SYSTEM/
│
├── backend/                      # Backend (Node.js + Express)
│   ├── config/                   # Database & app configuration
│   │   └── db.js
│   │
│   ├── controllers/              # Business logic
│   │   ├── authController.js
│   │   ├── employeeController.js
│   │   ├── leaveController.js
│   │   ├── salaryController.js
│   │   └── enquiryController.js
│   │
│   ├── middleware/               # Custom middlewares
│   │   ├── authMiddleware.js     # JWT verification
│   │   └── roleMiddleware.js     # Role-based access
│   │
│   ├── models/                   # MongoDB schemas
│   │   ├── User.js
│   │   ├── Employee.js
│   │   ├── Leave.js
│   │   ├── Salary.js
│   │   └── Enquiry.js
│   │
│   ├── routes/                   # API routes
│   │   ├── authRoutes.js
│   │   ├── employeeRoutes.js
│   │   ├── leaveRoutes.js
│   │   ├── salaryRoutes.js
│   │   └── enquiryRoutes.js
│   │
│   ├── uploads/                  # Uploaded files (PDFs)
│   │   └── salary-slips/
│   │
│   ├── utils/                    # Helper functions
│   │   └── pdfGenerator.js
│   │
│   ├── .env                      # Environment variables
│   ├── .gitignore
│   ├── package.json
│   ├── package-lock.json
│   └── server.js                 # Entry point
│
├── frontend/                     # Frontend (React)
│   ├── public/
│   │   └── index.html
│   │
│   ├── src/
│   │   ├── components/           # Reusable components
│   │   ├── pages/                # Pages (Admin, Employee)
│   │   │   ├── Login.jsx
│   │   │   ├── AdminDashboard.jsx
│   │   │   └── EmployeeDashboard.jsx
│   │   │
│   │   ├── services/             # API calls
│   │   │   └── api.js
│   │   │
│   │   ├── context/              # Auth & global state
│   │   ├── utils/
│   │   ├── App.js
│   │   └── index.js
│   │
│   ├── .gitignore
│   ├── package.json
│   └── package-lock.json
│
├── .gitignore                    # Root ignore file
├── README.md
└── LICENSE


---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js
- MongoDB
- Git

---

### 🔹 Backend Setup

```bash
cd backend
npm install
npm run dev
🔹 Frontend Setup
bash
Copy code
cd frontend
npm install
npm start
🔑 Environment Variables
Create a .env file in the backend folder:

env
Copy code
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
▶️ Usage
Start MongoDB

Run backend server

Run frontend application

Login as Admin or Employee

Manage ERP operations through dashboard

📈 Future Enhancements
Attendance management

Payroll automation

Performance tracking

Email notifications

Mobile app support

👨‍💻 Author
Suryanshu Kushwaha

GitHub: SuryanshuKushwaha

📜 License
This project is licensed under the MIT License.

yaml
Copy code

---

## ✅ Next Steps (Optional)
If you want, I can:
- Customize README **exactly to your backend/frontend code**
- Add **screenshots section**
- Add **API documentation**
- Create **deployment instructions (Render / Vercel)**

Just tell me 👍

