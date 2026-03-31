# ReqRes API Testing Project

## Overview

This project demonstrates API testing using Postman and Newman on the ReqRes public API.

## Scope

* Functional API testing (GET, POST, PUT, DELETE)
* Positive and negative test scenarios
* Request chaining (POST → PUT → DELETE)
* Environment-based variable handling
* API contract validation
* Basic performance validation (response time)

## Tools Used

* Postman
* Newman (CLI)
* htmlextra reporter

## Key Highlights

* Implemented dynamic request chaining using environment variables
* Validated API responses (status codes, structure, data types)
* Identified API defects (missing validation, invalid datatype handling)
* Generated automated HTML test reports using Newman

## Execution

Run the following command:

newman run ReqRes_API_Testing.postman_collection.json -e qa_environment.json -r cli,htmlextra --reporter-htmlextra-export report.html

## Note

ReqRes is a mock API; POST/PUT/DELETE operations do not persist data.
