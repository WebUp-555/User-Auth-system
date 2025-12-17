User Authentication System (Backend)

A backend authentication system implementing secure user login, token-based authentication, and protected routes. This project focuses on core auth functionality and is currently under development.


---

✅ Implemented Features

User registration with email & password

Secure password hashing using bcrypt

User login and logout

JWT-based authentication

Access tokens

Refresh tokens


Token verification middleware for protected routes

Secure cookie / header-based token handling (if used)



---

🛠 Tech Stack

Node.js

Express.js

MongoDB & Mongoose

JWT (Access & Refresh Tokens)

bcrypt



---

📁 Project Structure

auth-backend/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   └── app.js
├── .env
├── package.json
└── README.md


---

🔐 Authentication Flow

1. User registers with email and password


2. Password is hashed before storing in the database


3. User logs in using valid credentials


4. Server issues:

Access Token (short-lived)

Refresh Token (long-lived)



5. Protected routes validate access token via middleware




---

📡 API Endpoints (Current)

Auth

POST /api/v1/auth/register – Register user

POST /api/v1/auth/login – Login user

POST /api/v1/auth/logout – Logout user (token invalidation handled client-side or via refresh token logic)



---

⚙️ Environment Variables

PORT=8000
MONGODB_URI=your_mongodb_uri
ACCESS_TOKEN_SECRET=your_access_token_secret
REFRESH_TOKEN_SECRET=your_refresh_token_secret


---

▶️ Run Locally

npm install
npm run dev


Server runs locally at:
http://localhost:8000

---

🚧 Status

This authentication system is functional and extendable.
Planned improvements include:

Email verification

Forgot password flow

Role-based authorization



---

👨‍💻 Author

Shamsheer 
Backend Developer
