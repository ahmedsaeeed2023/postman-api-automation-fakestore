# API Test Automation – FakeStore API

## 📋 Overview
Automated API testing project built with **Postman** and **JavaScript assertions**, targeting the [FakeStore API](https://fakestoreapi.com/) — a public REST API used for e-commerce testing practice. Test collections are executed via **Newman** (Postman's CLI runner) to generate automated execution reports.

## 🎯 Objective
To design and automate API test scenarios that validate response structure, status codes, and business logic across FakeStore API endpoints (Products, Carts, Users), simulating real-world API test automation workflows.

## 🛠️ Tools & Techniques
- **Tool:** Postman
- **Assertions:** JavaScript (pm.test, pm.expect)
- **CLI Runner:** Newman
- **API Type:** RESTful (GET, POST, PUT, DELETE)

## ✅ Covered Test Scenarios
- Status code validation (200, 201, 404, etc.)
- Response schema & data type validation
- Business rule validation (e.g., price format, required fields)
- CRUD operations on Products/Carts/Users endpoints

## 📁 Project Structure
├── collections/
│   └── FakeStore_API_Collection.postman_collection.json
├── environments/
│   └── FakeStore.postman_environment.json
├── reports/
│   └── newman-report.html
└── README.md
## ▶️ How to Run
1. Import the collection and environment into Postman, **or**
2. Run via Newman CLI:
```bash
npm install -g newman
newman run collections/FakeStore_API_Collection.postman_collection.json -e environments/FakeStore.postman_environment.json -r html --reporter-html-export reports/newman-report.html
```

## 🔑 Key Skills Demonstrated
- API testing fundamentals (requests, headers, parameters, body)
- Writing JavaScript test assertions in Postman
- Environment variables for reusable, dynamic requests
- Automated execution & reporting with Newman
- Understanding RESTful services and status codes

---
**Author:** Ahmed Saeed Hemdan | [LinkedIn](https://www.linkedin.com/in/ahmed-saeed-hemdan/)
