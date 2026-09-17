# FastAPI Blog Project

A simple Blog API built using **FastAPI**, **SQLAlchemy**, and **PostgreSQL/SQLite**, supporting full CRUD operations, authentication, and pagination/search.

## 🚀 Live Demo

[https://fastapi-project-he1x.onrender.com](https://fastapi-project-he1x.onrender.com)

Interactive API docs: `/docs`

## 🛠️ Tech Stack

- **FastAPI** – Web framework
- **SQLAlchemy** – ORM for database operations
- **Pydantic** – Data validation
- **Uvicorn** – ASGI server
- **PostgreSQL / SQLite** – Database

## ✨ Features

- Create, Read, Update, Delete (CRUD) blogs
- Search and pagination support on blog listing
- User authentication (JWT-based)
- Auto-generated interactive API documentation (Swagger UI)
- Deployed on Render

## 📂 Project Structure

```
FastAPI-Project/
│
├── main.py          # Application entry point & API routes
├── models.py        # SQLAlchemy database models
├── schemas.py        # Pydantic request/response schemas
├── database.py       # Database connection & session setup
├── auth.py            # Authentication logic
├── requirements.txt   # Project dependencies
└── README.md
```

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ganesh-654-cpu/FastAPI_Project.git
   cd FastAPI_Project
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   venv\Scripts\activate      # Windows
   source venv/bin/activate   # Mac/Linux
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**

   Create a `.env` file in the root directory with the required variables (e.g. database URL, secret key).

5. **Run the application**
   ```bash
   uvicorn main:app --reload
   ```

6. **Open in browser**
   ```
   http://127.0.0.1:8000/docs
   ```

## 📌 API Endpoints

| Method | Endpoint       | Description         |
|--------|----------------|----------------------|
| GET    | `/`            | Health check         |
| POST   | `/blogs`       | Create a new blog    |
| GET    | `/blogs`       | Get all blogs (with search & pagination) |
| GET    | `/blogs/{id}`  | Get a single blog    |
| PUT    | `/blogs/{id}`  | Update a blog        |
| DELETE | `/blogs/{id}`  | Delete a blog        |

## 👤 Author

**Ganesh Mahajan**
GitHub: [@Ganesh-654-cpu](https://github.com/Ganesh-654-cpu)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).