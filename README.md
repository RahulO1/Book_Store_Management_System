# 📚 Bookstore Management System

A full-stack MERN (MongoDB, Express.js, React, Node.js) web application that allows admins and students to manage books, with secure login functionality and role-based access.

---

## 🚀 Features

- 🔐 Admin & Student login with JWT authentication  
- 📘 Add, view, edit, delete books  
- 📄 Role-based UI (Admin vs Student)  
- 🛠 Built with MongoDB, Express, React, and Node.js  
- 🌐 RESTful API structure  
- 🎨 Responsive and clean UI with CSS  
- ⚙️ Axios integration for frontend/backend communication  

---

## 📂 Project Structure

```
bookstore-management/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── db.js
│   ├── server.js
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── Login.jsx
│   └── public/
├── README.md
```

---

## 🧰 Tech Stack

| Layer     | Technology        |
|-----------|-------------------|
| Frontend  | React, Axios, CSS |
| Backend   | Express.js        |
| Database  | MongoDB, Mongoose |
| Auth      | bcrypt, JWT       |

---

## 📦 Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/bookstore-management.git
cd bookstore-management
```

### 2️⃣ Setup Backend
```bash
cd backend
npm install
cp .env.example .env
# Edit .env with your Mongo URI and JWT secret
npm run dev
```

### 3️⃣ Setup Frontend
```bash
cd ../frontend
npm install
npm run dev  # or npm start if using CRA
```

---

## 🌍 Environment Variables

Create a `.env` file in `/backend/` with the following:

```env
PORT=3001
MONGO_URI=mongodb://localhost:27017/bookstore
JWT_SECRET=your_jwt_secret
```

---

## 🔐 Sample Admin Creation

To generate the first admin:

```bash
node createAdmin.js
```

Or call `Admin.create()` manually with hashed password using bcrypt.

---

## 📮 API Endpoints

### Authentication
| Route         | Method | Description                |
|---------------|--------|----------------------------|
| `/auth/login` | POST   | User login (admin/student) |

### Books
| Route           | Method | Description         |
|------------------|--------|---------------------|
| `/books`         | GET    | Fetch all books     |
| `/books/:id`     | GET    | Get book by ID      |
| `/books`         | POST   | Add a new book      |
| `/books/:id`     | PUT    | Edit book           |
| `/books/:id`     | DELETE | Delete book         |

---

## 🧪 Testing

You can use **Postman** or **Thunder Client** to test APIs.

---

## 📸 Screenshots

> Add screenshots of your login page, book list, and admin dashboard here.

---

## 🧑‍💻 Author

- Name: [Your Name]  
- GitHub: [@your-username](https://github.com/your-username)  
- Email: your@email.com

---

## 📜 License

This project is licensed under the MIT License. Feel free to use and modify it.
