# ReqRes API Testing – Postman + Newman

## 📌 Project Overview

This project demonstrates API testing of the public ReqRes API using Postman and Newman. It focuses on functional validation, response structure verification, status code validation, and negative test scenarios.

The goal is to simulate real-world backend API testing and showcase practical QA skills relevant for entry-level testing roles.

---

## 🧪 API Endpoints Covered

* Authentication (Login / Register)
* GET Users (List Users, Single User)
* POST (Create User)
* PUT (Update User)
* DELETE (Delete User)

---

## ✅ Test Scenarios Covered

* Validate successful user retrieval (GET) returns 200 with correct data
* Validate single user endpoint returns expected user details
* Validate user creation (POST) returns 201 and correct response body
* Validate update operation (PUT) reflects updated data
* Validate delete operation returns 204 with no content
* Validate unsuccessful login returns 400 with appropriate error message
* Verify response time is within acceptable limits (<1000ms)
* Validate response structure and key response fields

---

## 🛠 Tools Used

* Postman (API Testing)
* Newman (Command-line execution)
* HTML Reporter (Test execution reports)
* JavaScript (Postman test scripts)

---

## 📂 Project Structure

* `collections/` → Postman collection files
* `environments/` → Environment configuration files
* `reports/` → Generated Newman reports (not stored in repository)

---

## ▶️ How to Run the Tests

### Using Postman

1. Import the collection and environment files
2. Select the appropriate environment
3. Run using Collection Runner

### Using Newman

```bash
newman run collections/ReqRes_API_Testing.postman_collection.json -e environments/qa_environment.json -r html
```

---

## 📊 Sample Test Script

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains expected data", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.data).to.exist;
});
```

---

## 📊 Test Execution

HTML reports are generated using Newman during execution.

Note: Reports are dynamically generated and not stored in the repository.

---

## 🎯 Key Highlights

* End-to-end API testing using Postman and Newman
* Implementation of both positive and negative test scenarios
* Automated test execution with HTML reporting
* Validation of response data, status codes, and performance
* Structured and maintainable test collection design

---

## 🚀 Future Improvements

* Integrate API tests with CI/CD tools (e.g., GitHub Actions)
* Add JSON schema validation for response structure verification
* Implement data-driven testing using external data files
* Enhance negative test coverage for edge cases
* Support multiple environments (Dev, QA, Prod)

---

## 🔗 API Reference

https://reqres.in


---

## 👩‍💻 Author

 Janani Jayarajan
 QA Engineer |  ISTQB CTFL Certified | AT\*SQA AT\*API Certified 


