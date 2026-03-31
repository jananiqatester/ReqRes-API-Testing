# ReqRes API Testing Project

## 📌 Project Overview

This project demonstrates API testing of the public ReqRes API using Postman. It covers functional validation, status code verification, and basic contract checks.

The goal of this project is to simulate real-world API testing scenarios and showcase QA skills relevant for backend testing roles.

---

## 🧪 Scope of Testing

* Authentication APIs
* GET (List Users, Single User)
* POST (Create User)
* PUT (Update User)
* DELETE (Delete User)

---

## ⚙️ Tools Used

* Postman
* Newman (CLI execution)
* HTML Reporter

---

## 📂 Project Structure

* `collections/` → Postman collection files
* `environments/` → Environment configuration
* `reports/` → Generated reports (ignored in Git)

---

## ✅ Test Coverage

* Status code validation (200, 201, 204, etc.)
* Response body validation
* Data consistency checks
* Negative scenarios (invalid inputs)

---

## ▶️ How to Run

### Using Postman

1. Import collection and environment
2. Run using Collection Runner

### Using Newman

```
newman run collections/ReqRes_API_Testing.postman_collection.json -e environments/qa_environment.json -r html
```

---

## 📊 Test Execution

HTML report is generated using Newman during test execution.

> Note: Reports are dynamically generated and not stored in the repository.

---

## 🎯 Key Highlights

* Structured API test cases
* Real-world API testing scenarios
* Clean project organization
* Command-line test execution using Newman

---

## 🚀 Future Improvements

* Integrate API tests with CI/CD tools like GitHub Actions
* Add JSON schema validation for response structure verification
* Implement data-driven testing using external data files
* Enhance negative test coverage for edge cases
* Support multiple environments (Dev, QA, Prod)

---

## 👩‍💻 Author

 Janani Jayarajan
 QA Engineer |  ISTQB CTFL Certified | AT\*SQA AT\*API Certified 


