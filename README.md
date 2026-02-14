# backend-java-assignment-Spring Boot Backend

## 📌 Project Overview
This is a simple RESTful API built using Spring Boot that manages a collection of items.
The application uses in-memory storage (ArrayList) and supports adding and retrieving items.

---

## 🚀 Tech Stack
- Java 17+
- Spring Boot
- Maven
- Lombok
- Jakarta Validation

---

## 📂 Features Implemented

1. Item Model with fields:
   - id
   - name
   - description
   - price

2. In-memory data storage using ArrayList

3. REST API Endpoints:
   - Add a new item
   - Get item by ID

4. Input validation using Jakarta Validation

5. Global exception handling for validation errors

---

## 🔗 API Endpoints

### 1️⃣ Add Item

POST /api/items

Request Body:
{
  "name": "Laptop",
  "description": "Gaming Laptop",
  "price": 75000
}

Response:
201 CREATED

---

### 2️⃣ Get Item by ID

GET /api/items/{id}

Example:
GET /api/items/1

Response:
200 OK

---

## ▶️ How to Run Locally

1. Clone the repository
2. Run:

mvn clean install  
mvn spring-boot:run  

OR run ItemsApiApplication from IDE.

Application runs at:
http://localhost:8080

---

## ⚠️ Important Notes
- Data is stored in memory and will reset when application restarts.
- No database is used as per assignment requirement.
