# 🔐 Node Auth App

A secure authentication system built with **Node.js, Express.js, MongoDB, and JWT**, featuring user registration, login, password hashing, and protected routes.

---

## 🚀 Features

- User registration and login system  
- Password hashing using **bcrypt**  
- Authentication using **JWT (JSON Web Tokens)**  
- Protected routes with middleware  
- RESTful API architecture  
- MongoDB database integration  
- Error handling and validation  

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (Mongoose ODM)  
- **Authentication:** JWT, bcrypt  
- **Other Tools:** dotenv, nodemon  

---

## 📁 Project Structure

node-auth-app/
│
├── routes/          # API routes
├── models/          # Mongoose schemas
├── middleware/      # Auth middleware
├── controllers/     # Business logic
├── config/          # Database configuration
├── .env             # Environment variables
├── server.js        # Entry point
└── package.json


---

## ⚙️ Installation

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/KAB145/node-auth-app.git
cd node-auth-app
```
### 2. Install dependencies
npm install

### 3. Create a .env file

Add the following variables:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

## 4. Start the server
npm run dev

or

npm start

---

## 🔑 API Endpoints

### Auth Routes

| Method | Endpoint              | Description          |
|--------|---------------------|----------------------|
| POST   | /api/auth/register   | Register a new user  |
| POST   | /api/auth/login      | Login user           |

### Protected Route

| Method | Endpoint           | Description                                      |
|--------|------------------|--------------------------------------------------|
| GET    | /api/protected    | Access protected data (requires token)           |

---

## 🔒 Authentication Flow

- User registers → password is hashed using bcrypt  
- User logs in → credentials are validated  
- Server generates a JWT token  
- Client stores token and sends it in headers  
- Middleware verifies token for protected routes  

---

## 🧪 Testing with Postman
Register user via /api/auth/register
Login via /api/auth/login
Copy the returned token
Add header:
Authorization: Bearer <your_token>

---

## 📌 Future Improvements
Email verification
Password reset functionality
Role-based authorization (admin/user)
Refresh tokens
OAuth (Google/GitHub login)

---

## 👨‍💻 Author

- GitHub: [KAB145](https://github.com/KAB145)
