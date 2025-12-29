# DummyJSON API Testing Pack

A Postman API testing collection built for QA practice and portfolio purposes.  
It demonstrates positive and negative testing with reusable environment variables and automated assertions, making it portfolio-ready.

---

## Collection Overview

This collection covers:

- **Authentication** – Login (valid & invalid scenarios)
- **Users** – Retrieve user lists and individual users (valid & invalid scenarios)  
- **Posts** – Retrieve posts (valid & invalid scenarios)

Each request includes:

- Proper HTTP method  
- Test scripts for status code verification  
- Assertions for response body validation  
- Environment variables for easy reusability  

---

## Folder Structure

DummyJSON API Testing Pack
├── Authentication
│ ├── Login – Valid Credentials
│ ├── Login – Invalid Credentials
├── Users
│ ├── Get Users – Valid
│ ├── Get Single User – Valid
│ └── Get Single User – Invalid
└── Posts
  ├── Get Posts – Valid
  └── Get Post – Invalid

---

## Environment Variables

**Environment Name:** `DummyJSON_Env`

| Variable   | Value                  | Description                 |
|-----------|-----------------------|----------------------------|
| base_url  | https://dummyjson.com  | Base URL for API requests   |

Using environment variables allows you to reuse requests across different environments.

---

## How to Use

1. Import the collection into Postman Web: [https://web.postman.co](https://web.postman.co)  
2. Create or import the environment `DummyJSON_Env` and set `base_url`.  
3. Select the collection → select a request → click **Send**.  
4. Observe the response and test results in the **Tests** tab.  

---

## Positive & Negative Testing Examples

**Authentication**

- Positive: `Login - Valid Credentails` → Status 200, returns user information with access token
- Negative: `Login - Invalid Credentails` → Status 400, error message present

**Users**

- Positive: `Get Users – Valid` → Status 200, returns an array of users  
- Negative: `Get Single User – Invalid` → Status 404, error message present  

**Posts**

- Positive: `Get Posts – Valid` → Status 200, returns an array of posts  
- Negative: `Get Post – Invalid` → Status 404, error message present  

These requests and tests showcase practical QA skills: designing positive and negative scenarios, writing assertions, and handling edge cases.

---

## Author

**Samina Moiyadi** – ISTQB Advanced-certified QA professional building portfolio-ready assets.
