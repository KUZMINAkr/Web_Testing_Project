# 📚 Web Testing Project — BookStore API & UI Testing  
Comprehensive QA project including API testing, UI validation, bug reports, and documentation.

---

## 🚀 Project Overview  
This project demonstrates practical QA skills through testing the **BookStore API** and UI components at **demoqa.com**.  
Includes:  
- API testing (positive + negative cases)  
- UI testing  
- Bug reports with severity & priority  
- Screenshots  
- Structured documentation

---

# 🧪 API Test Cases (BookStore API)

### **TC_API_001 — Create User (Positive)**  
**Precondition:** Username does not exist  
**Steps:**  
1. Send POST `/User` with valid body  
**Expected Result:** `201 Created`, userID returned

---

### **TC_API_002 — Create User (Negative: Weak Password)**  
**Steps:**  
1. Send POST `/User` with password `"123"`  
**Expected Result:** `400 Bad Request`, password validation error

---

### **TC_API_003 — Generate Token**  
**Expected Result:**  
`200 OK`, token generated

---

### **TC_API_004 — Authorization Check**  
**Expected Result:**  
Response: `"result": true`

---

### **TC_API_005 — Add Book to Collection**  
**Expected Result:** `201 Created`

---

### **TC_API_006 — Delete Book**  
**Expected Result:** `204 No Content`

---

# 🐞 Bug Tracking Table  

| Bug ID | Title | Severity | Priority | Status |
|-------|--------|----------|----------|--------|
| **B001** | WebTables loads empty | High | High | Open |
| **B002** | Book page shows white screen | High | High | Open |
| **B003** | Radio button “No” disabled | Medium | Medium | Open |
| **B004** | Slider drag incorrect | Medium | Low | Open |
| **B005** | Grid items stick to cursor | Low | Low | Open |
| **B006** | List items stick to cursor | Low | Low | Open |
| **B007** | “More” menu inactive | Medium | Low | Open |
| **B008** | Resizable box jumps, incorrect size limits | Medium | Low | Open |

---

# 🎨 UI Testing Checklist  

## ✓ General UI  
- [x] Page loads correctly  
- [x] Text readable  
- [x] No broken elements  
- [x] Buttons clickable  
- [x] Hover states visible  

## ✓ Interactive Elements  
- [x] Slider movement  
- [x] Draggable elements  
- [x] Selectable items  
- [x] Resizable box  
- [x] Tabs switching  

---

# 📂 Project Structure  

Web_Testing_Project/
│
├── screenshots/
│ ├── API/
│ ├── Bugs/
│ ├── UI/
│
├── README.md
└── other documentation files

yaml
Copy code

---

# ✨ Additional QA Documentation

This project also includes:

### ✔ Full API Test Cases  
(see above)

### ✔ Complete Bug Table  
(with severity & priority)

### ✔ UI Testing Checklist  
(validated components, interactions, and visual elements)

---

# 🧾 Final Notes  
This project demonstrates my ability to:

- analyze API behavior  
- identify UI problems  
- write clean bug reports  
- structure QA documentation  
- organize testing work for a portfolio-ready project  

---

# 👩‍💻 Author  

**Karina Kuzmina**  
Aspiring QA Engineer / Future Backend Developer  
