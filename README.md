# 📦 MongoDB-API

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A Python-based REST API that provides CRUD operations on a MongoDB database. This project demonstrates how to build a lightweight backend service using Python and MongoDB.

---

## 🧠 Problem Statement

Applications often require a simple and scalable backend to manage data. This project exposes MongoDB operations via RESTful APIs for easy integration with any frontend or client.

---

## 🏗️ Architecture

Client → Flask/FastAPI → PyMongo → MongoDB

---

## ✨ Features

- RESTful CRUD APIs  
- MongoDB integration using PyMongo  
- Environment-based configuration with `.env`  
- Modular and clean codebase  

---

## 🛠️ Tech Stack

- Python  
- Flask / FastAPI  
- MongoDB  
- PyMongo  
- python-dotenv  

---

## 📂 Project Structure

MongoDB-API/
├── app.py
├── requirements.txt
├── .env.example
├── routes/
├── models/
└── README.md


---

## ⚙️ Environment Variables

Create a `.env` file in the root directory:

```env
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/dbname


🚀 Installation

git clone https://github.com/shauryananda3/MongoDB-API.git
cd MongoDB-API
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt

▶️ Run the Application

python app.py

🔌 API Endpoints

| Method | Endpoint    | Description      |
| ------ | ----------- | ---------------- |
| GET    | /items      | Fetch all items  |
| POST   | /items      | Create new item  |
| GET    | /items/<id> | Fetch item by ID |
| PUT    | /items/<id> | Update item      |
| DELETE | /items/<id> | Delete item      |

📋 Example Request

curl -X POST http://localhost:5000/items \
-H "Content-Type: application/json" \
-d '{"name":"Laptop","price":75000}'

👤 Author
Shaurya Nanda
🔗 LinkedIn: https://www.linkedin.com/in/shaurya-nanda

