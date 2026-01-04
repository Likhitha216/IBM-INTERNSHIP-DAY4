# IBM-INTERNSHIP-DAY4

📚 Library Management System (Node.js + MongoDB)

A simple and powerful Library Management System REST API built using Node.js, Express, and MongoDB.
This project demonstrates CRUD operations, database integration, and clean API design — perfect for students, beginners, and portfolio projects.

✨ Features

✅ Add multiple books to the library
✅ View all books
✅ Filter books by category
✅ Get books published after a specific year
✅ Update available copies (increase/decrease stock)
✅ Change book category
✅ Delete a book only when copies are 0
✅ MongoDB integration using Mongoose

🛠️ Tech Stack

Backend: Node.js, Express.js

Database: MongoDB

ODM: Mongoose

API Style: RESTful APIs

📂 Project Structure
📁 Library-Management-System
│
├── app.js           # Main server file & API routes
├── db.js            # MongoDB connection
├── bookmodel.js     # Book schema & model
├── package.json     # Dependencies
└── package-lock.json

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/library-management-system.git

2️⃣ Navigate to the project folder
cd library-management-system

3️⃣ Install dependencies
npm install

4️⃣ Start MongoDB

Make sure MongoDB is running locally on:

mongodb://127.0.0.1:27017/libraryDB

5️⃣ Run the server
node app.js


🚀 Server will start on:

http://localhost:3000

📌 API Endpoints
➕ Add Books (Insert 7 default books)

POST

/addBooks

📖 Get All Books

GET

/books

📂 Get Books by Category

GET

/books/category/:category


Example:

/books/category/AI

📅 Get Books Published After 2015

GET

/books/year/after2015

🔄 Update Available Copies

PUT

/books/updateCopies/:id


Body:

{
  "change": 2
}

🏷️ Change Book Category

PUT

/books/changeCategory/:id


Body:

{
  "category": "Programming"
}

🗑️ Delete Book (Only if copies = 0)

DELETE

/books/delete/:id

🧠 Learning Outcomes

CRUD operations using MongoDB

REST API design with Express

Mongoose schema & validation

Error handling in backend APIs

Real-world backend project structure

🚀 Future Enhancements

🔹 User authentication (Admin / Student)
🔹 Borrow & Return books feature
🔹 Frontend using React
🔹 Search & pagination
🔹 Deployment on Render / Railway

👩‍💻 Author

VAJJA LIKHITHA (AI & DS Student)
📌 Beginner-friendly backend project for learning & practice
