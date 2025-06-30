# 📝 TechNotes API

**TechNotes API** is a backend service built with **Node.js** and **Express.js**, providing a RESTful interface for managing users and their notes. It supports user authentication, note creation, updating, and deletion—ideal for use in productivity apps or admin dashboards.

---

## 🚀 Features

- 🔐 User authentication with **JWT**
- 🗒️ Full CRUD operations for notes
- 👤 User roles and permission control
- 🧼 Clean architecture with MVC pattern
- ✅ Request validation and error handling middleware

---

## 🛠️ Tech Stack

- **Runtime**: Node.js  
- **Framework**: Express.js  
- **Database**: MongoDB with Mongoose  
- **Authentication**: JSON Web Tokens (JWT)  
- **Other Tools**: Dotenv, CORS, Morgan

---

## 📦 Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/symon9/technotes-api.git
   cd technotes-api
   ```

2. **Install dependencies**  
   ```bash
   npm install
   ```

3. **Set up environment variables**  
   Create a `.env` file in the root and add:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   ACCESS_TOKEN_SECRET=your_jwt_secret
   ```

4. **Run the app locally**  
   ```bash
   npm run dev
   ```

   The server will start at `http://localhost:5000`.

---

## 📁 Folder Structure

```
.
├── config/          # Database and app config
├── controllers/     # Route logic
├── middleware/      # Auth, error handling, etc.
├── models/          # Mongoose schemas
├── routes/          # API route definitions
├── utils/           # Helper functions
├── .env             # Environment variables
├── server.js        # App entry point
└── package.json
```

---

## 🧭 API Overview

| Method | Endpoint           | Description             |
|--------|--------------------|-------------------------|
| POST   | /auth              | Login user              |
| GET    | /users             | Get all users (admin)   |
| POST   | /users             | Create new user         |
| PATCH  | /users/:id         | Update user info        |
| DELETE | /users/:id         | Delete user             |
| GET    | /notes             | Get all notes           |
| POST   | /notes             | Create a new note       |
| PATCH  | /notes/:id         | Update a note           |
| DELETE | /notes/:id         | Delete a note           |

> ⚠️ Some routes require admin access or JWT authentication.

---

## 🌐 Deployment

- Ready for deployment on platforms like **Render**, **Vercel (Serverless Functions)**, or **Railway**.
- Be sure to configure your production `.env` file accordingly.

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to change.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 📌 Author

Made with ❤️ by [symon9](https://github.com/symon9)
