# API Testing - User Creation Validation

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pytest](https://img.shields.io/badge/Tested%20With-Pytest-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![QA](https://img.shields.io/badge/Focus-QA%20Automation-orange)

This project contains automated API tests focused on validating the `firstName` parameter when creating a user.

Designed and implemented as part of a QA Automation workflow, this project simulates real-world API validation scenarios, ensuring data integrity and proper error handling.

---

## 📌 Overview

This test suite validates multiple scenarios for user creation, focusing on input validation and API response behavior.

Key scenarios covered:

* Valid user creation
* Invalid input formats
* Boundary value analysis
* Missing or null fields
* Negative testing scenarios

---

## 🛠️ Tech Stack

* Python 🐍
* Pytest ⚡
* Requests 🌐

---

## 💼 Professional Context

This project reflects practical QA Automation skills applicable in real-world environments:

* API validation using automated tests
* Test case design based on input validation rules
* Separation of concerns (data, configuration, request handling)
* Structured and maintainable test code
* Simulation of backend validation scenarios

---

## 📂 Project Structure

```bash
api_stand_test/
│
├── main.py                     # Entry point (if applicable)
├── configuration.py           # Environment configuration
├── sender_stand_request.py    # API request handler
├── data.py                    # Test data definitions
├── create_user_test.py        # Test cases
│
└── resources/
    └── data.txt               # Supporting data
```

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/Fitzonder/api_stand_test.git
cd api_stand_test
```

2. Install dependencies:

```bash
pip install pytest requests
```

---

## ▶️ Running Tests

Execute all tests with:

```bash
pytest
```

For more detailed output:

```bash
pytest -v
```

---

## 🧪 Example API Test Scenario

### 🔹 Request

```json
POST /users
{
  "firstName": "Carlos"
}
```

### 🔹 Expected Response

```json
{
  "status": "success",
  "message": "User created successfully"
}
```

---

### 🔹 Negative Test Example

```json
POST /users
{
  "firstName": ""
}
```

### 🔹 Expected Response

```json
{
  "status": "error",
  "message": "firstName cannot be empty"
}
```

---

## 📈 Key Testing Validations

* Response status code verification
* Input validation logic
* Error handling verification
* Data-driven testing approach
* Boundary value analysis

---

## 🚧 Future Improvements

* Add validation for additional fields (lastName, email)
* Implement test parameterization with pytest
* Integrate Allure Reports for advanced reporting
* Add CI/CD pipeline with GitHub Actions
* Environment-based configuration (dev/staging)

---

## 👨‍💻 Author

Carlos Lenis
QA Automation Engineer (Junior) 🚀

---

## 📬 Contact

If you're a recruiter or hiring manager, feel free to connect:

* LinkedIn: *https://www.linkedin.com/in/carlos-lenis-812a5918/*
* GitHub: https://github.com/Fitzonder


