## 📘 Student Management REST API

A backend **RESTful API** built using **Django REST Framework** to manage student records with full CRUD functionality.  
The project demonstrates clean API design, proper HTTP methods, status codes, and API testing using Postman.

---

## 🚀 Features

- Create a new student
- Retrieve all students
- Retrieve a single student by ID
- Update student details
- Delete a student
- Proper HTTP status codes (`200`, `201`, `204`, `404`)
- JSON-based API responses

---

## 🛠️ Tech Stack

- **Backend:** Python, Django
- **API Framework:** Django REST Framework (DRF)
- **Database:** SQLite (default Django DB)
- **API Testing:** Postman
- **Version Control:** Git & GitHub

---

## 📂 Project Structure

```text
student_api/
│
├── config/              # Project settings & URLs
├── students/            # Student app (models, views, serializers)
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│
├── manage.py
├── requirements.txt
├── .gitignore
```

## 🔗 API Endpoints

Base URL
```
http://127.0.0.1:8000/api/
```
| Method | Endpoint          | Description       |
| ------ | ----------------- | ----------------- |
| GET    | `/students/`      | Get all students  |
| POST   | `/students/`      | Add a new student |
| GET    | `/students/<id>/` | Get student by ID |
| PUT    | `/students/<id>/` | Update student    |
| DELETE | `/students/<id>/` | Delete student    |

---  

## 📦 Sample Request (POST)

```
{
  "name": "Anushka",
  "age": 22,
  "email": "anu@gmail.com",
  "course": "Django",
  "grade": "A"
}
```
---

## 📤 Sample Response
```
{
  "id": 1,
  "name": "Anushka",
  "age": 22,
  "email": "anu@gmail.com",
  "course": "Django",
  "grade": "A"
}
```
---

## ▶️ How to Run the Project Locally
- 1️⃣ Clone the repository
```
git clone https://github.com/anushkapundir1/student-management-api.git
cd student-management-api
```
- 2️⃣ Create and activate virtual environment
```
python -m venv venv
venv\Scripts\activate   # Windows
```
- 3️⃣ Install dependencies
```
  pip install -r requirements.txt
```
- 4️⃣ Run migrations
```
python manage.py makemigrations
python manage.py migrate
```
- 5️⃣ Start the server
```
python manage.py runserver
```
---
## 🧪 API Testing
All endpoints were tested using Postman, ensuring correct request handling and responses.

---

## 📌 Learning Outcomes

- Understanding REST API architecture

- Working with Django REST Framework

- Implementing CRUD operations

- Using serializers for JSON conversion

- Following clean GitHub version control practices
 
---

## 👩‍💻 Author

Anushka Pundir





