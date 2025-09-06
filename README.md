# 📝 Node.js + MongoDB Authentication API

Welcome to this simple **Auth API** built with Node.js, Express, MongoDB, Bcrypt & JWT! 🔥

---

## ⚡ Features
- ✅ Register a user
- ✅ Login a user
- ✅ Password hashing with **Bcrypt**
- ✅ JWT token generation
- 🛠 Built with **Node.js** & **MongoDB**

---

## 🚀 Installation

1. Clone the repository

git clone https://github.com/FaeizHamdard22/node.js-register-login.git
cd node.js-register-login
Install dependencies


npm install
Create a .env file in the root:


MONGO_URI="mongodb://localhost:27017/your-db-name"
PORT=5000
JWT_SECRET="your_secret_key"
Run the server


node app.js
Server will start on http://localhost:5000 🎉

🔗 API Endpoints
1️⃣ Register User
POST /api/auth/register

Body (JSON):

{
  "username": "faeiz",
  "email": "faeizhamdard48.com",
  "password": "123456"
}
Response:


{
  "message": "Successfully registered"
}
2️⃣ Login User
POST /api/auth/login

Body (JSON):

{
  "email": "faeizhamdrd48@gmail.com,
  "password": "123456"
}
Response:

{
  "message": "Login successful",
  "token": "JWT_TOKEN_HERE"
}
⚠️ Use this token for authentication in other endpoints.

🧪 Testing with Postman
Open Postman 🔹

Create a new POST request

Set the URL:

http://localhost:5000/api/auth/register
Set Body to raw JSON and add the fields:

{
  "username": "faeiz",
  "email": "faeizhamdard48@gmail.com",
  "password": "123456"
}
Hit Send ✅

You should see:

{
  "message": "Successfully registered"
}
For login, do the same with /api/auth/login endpoint.

👏 Notes
Make sure MongoDB is running locally.

Do not push node_modules/ to GitHub, it's ignored via .gitignore.

Passwords are automatically hashed using bcrypt 🔐

Tokens expire in 1 hour ⏱

💡 Enjoy testing your API! 🚀
