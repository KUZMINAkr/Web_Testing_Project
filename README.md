# Web & API Testing Project  
A complete QA portfolio project demonstrating manual UI testing, API testing, bug reporting, and technical documentation skills.

---

## 📌 Project Overview  
This project includes UI testing of **demoqa.com** and API testing of the **BookStore API**.  
It demonstrates my ability to:

- Analyze API behavior  
- Detect UI defects  
- Write structured test cases  
- Create clear bug reports  
- Organize documentation professionally  

---

# 🧪 API Testing — BookStore API

All API tests were executed using **Postman** and manual exploration.

## ✔ 1. User Registration  
**Endpoint:** `POST /Account/v1/User`  
**Checks performed:**  
- User creation with valid data  
- Validation error when password does not meet requirements  
- Server response time & structure  

---

## ✔ 2. Authorization & Token  
**Endpoint:** `POST /Account/v1/GenerateToken`  
**Checks:**  
- Token generated successfully with valid credentials  
- Token status becomes `"Authorized"`  

---

## ✔ 3. Get User Data  
**Endpoint:** `GET /Account/v1/User/{UUID}`  
**Checks:**  
- Correct user information returned  
- Unauthorized access blocked  

---

## ✔ 4. Books — CRUD Testing  
### Add Book  
`POST /BookStore/v1/Books`  
### Get Book  
`GET /BookStore/v1/Book`  
### Delete Book  
`DELETE /BookStore/v1/Book`  

Checks include:  
- Valid ISBN handling  
- Error messages for invalid or missing ISBN  
- Successful book deletion  

---

# 🖼 Screenshots  
Screenshots for API tests are stored in:  
📁 `./screenshots`

---

# 🐞 Bug Reports (UI)  
All UI defects found on **demoqa.com** are located in:  
📁 `./bug_reports`

Each bug includes:  
- Title  
- Environment  
- Steps to reproduce  
- Expected result  
- Actual result  
- Severity & priority  
- Screenshot

---

# 📋 Additional QA Documentation

Below is structured documentation for this project.

---

# ✔ Test Cases — BookStore API

### 1. Create User

| Step | Input | Expected Result |
|------|--------|----------------|
| 1 | Send POST /Account/v1/User with valid data | 201 Created, userId returned |
| 2 | Send POST with weak password | 400 Bad Request, validation message |

---

### 2. Token Generation

| Step | Input | Expected Result |
|------|--------|----------------|
| 1 | Valid username & password | Token generated, status = Authorized |
| 2 | Invalid credentials | Token not issued |

---

### 3. Book Operations

| Case | Action | Expected |
|------|--------|----------|
| Add book | Send valid ISBN | 201 Created |
| Invalid ISBN | Send wrong ISBN | 400 Bad Request |
| Delete | Remove book by correct ISBN | 204 No Content |

---

# 🐞 Bug Tracking Table

| Bug ID | Title | Severity | Priority | Status |
|--------|--------|----------|----------|--------|
| 001 | WebTables not loading | High | High | Open |
| 002 | Incorrect redirect on Books page | Medium | Medium | Open |
| 003 | Radio button "Impressive" always selected | Low | Low | Open |
| 004 | Sortable grid elements float incorrectly | Medium | Medium | Open |
| 005 | Tabs content overflow | Low | Low | Open |

---

# 🎨 UI Testing Checklist

## ✓ General UI  
- [x] Page loads correctly  
- [x] All text is readable  
- [x] No broken elements  
- [x] Buttons clickable  
- [x] Hover states visible  

## ✓ Interactive Elements  
- [x] Slider movement  
- [x] Sortable lists  
- [x] Resizable boxes  
- [x] Tabs content switches  

---

# 🧾 Final Notes  
This project strengthened my ability to:

- Test REST APIs  
- Detect UI issues  
- Document QA artifacts professionally  
- Work with Postman  
- Create a real portfolio-ready QA project  

---

# 👩‍💻 Author  
**Karina Kuzmina**  
Aspiring QA Engineer | Future Backend Developer  
