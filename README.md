Fullstack MERN Assignment – Book Review Platform
A comprehensive Book Review Platform built with the MERN stack (MongoDB, Express, React, Node.js). Users can sign up, log in, add books, and review books. This app demonstrates skills in authentication, CRUD operations, protected routes, ratings, and pagination.

🚀 Features
User authentication (JWT tokens & password hashing)

Create, Read, Update, Delete (CRUD) for books

User book reviews with ratings and comments

Protected API routes and frontend pages

Average rating calculation per book (live)

Pagination for the book list (5 books per page)

MongoDB Atlas integration (production ready)

Proper schema design with Mongoose

🛠️ Tech Stack
React

Node.js

Express.js

MongoDB & Mongoose

JWT (jsonwebtoken)

bcrypt

📂 Folder Structure
text
/backend
    /config
    /controllers
    /middleware
    /models
    /routes
    .env
    server.js
    package.json

/frontend
    /src
        /api
        /components
        App.js
        index.js
    package.json
🚦 Getting Started
Prerequisites
Node.js & npm

MongoDB Atlas or local MongoDB

Setup Instructions
Clone the repository

text
git clone https://github.com/your-username/mern-book-review-platform.git
cd mern-book-review-platform
Backend Setup

bash
cd backend
npm install
# Create a .env file with:
# MONGO_URI=your_mongodb_url
# JWT_SECRET=your_secret_key
npm start
Frontend Setup

bash
cd ../frontend
npm install
npm start
Default backend: http://localhost:5000
Default frontend: http://localhost:3000

🌍 MongoDB Cloud Setup
Use MongoDB Atlas for cloud database.

Create a cluster, add a database user, and whitelist your IP.

Get your connection URL (MONGO_URI).

📜 API Routes
POST /api/auth/signup — Register user

POST /api/auth/login — Login user

GET /api/books — Get book list (pagination)

POST /api/books — Add book (auth required)

GET /api/books/:id — Book details + reviews

PUT /api/books/:id — Update book (auth/owner)

DELETE /api/books/:id — Delete book (auth/owner)

POST /api/books/:bookId/reviews — Add book review (auth required)
