# Postman API Integration & Error Handling

## Overview

This project demonstrates practical API integration and error-handling skills using Postman. It is designed to showcase how to work with REST APIs, validate responses, and handle common failure scenarios in a clear, structured, and repeatable way.

The collection uses a public REST API so it can be easily imported and tested by recruiters, engineers, or hiring managers without additional setup.

---

## Why This Project

Many API issues in real-world systems are not about complex logic, but about reliability, validation, and handling edge cases. This project focuses on:

* Making clean API requests
* Validating responses
* Identifying and handling common API errors
* Organizing requests in a way that reflects real testing workflows

---

## Tools Used

* Postman
* Public REST API (JSONPlaceholder)

---

## Scenarios Covered

### 1. API Integration (Happy Path)

These scenarios validate successful API communication and data handling.

**GET – Fetch All Posts**

* Retrieves a list of posts from the API
* Validates status code 200
* Confirms response structure is an array

**POST – Create New Post**

* Sends a JSON payload to create a new resource
* Validates status code 201
* Confirms returned object contains expected fields

Why this matters:
Demonstrates the ability to consume APIs, send structured data, and validate expected responses.

---

### 2. API Error Handling

These scenarios focus on how APIs behave when something goes wrong.

**GET – Invalid Endpoint (404)**

* Calls a non-existent endpoint
* Validates status code 404

**POST – Missing Required Fields**

* Sends an incomplete request body
* Validates client-side error response (400 or 422)

Why this matters:
Shows awareness that API testing is not just about success cases, but also about identifying and validating failures.

---

### 3. Data Validation

**Response Schema Validation**

* Confirms key fields exist in responses
* Validates data types where applicable

Why this matters:
Ensures downstream systems can rely on consistent and predictable API responses.

---

## Collection Structure

```
api-integration-and-error-handling
│
├── API Integration
│   ├── GET - Fetch All Posts
│   └── POST - Create New Post
│
└── API Error Handling
    ├── GET - Invalid Endpoint
    └── POST - Missing Required Fields
```

### Sample Requests

![GET Success](screenshots/get-fetch-all-posts-200.png)
![404 Error](screenshots/get-invalid-endpoint-404.png)
![POST Request](screenshots/post-create-new-post-response.png)


## How to Run This Project

1. Clone or download this repository
2. Open Postman
3. Import the collection file:
   `api-integration-error-handling.postman_collection.json`
4. Run requests individually or use the Collection Runner

No authentication or environment variables are required.




