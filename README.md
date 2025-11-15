🌐 Web & API Testing Project — DemoQA

By Karina Kuzmina

This project demonstrates manual API testing, UI functional testing, and bug reporting skills using DemoQA’s BookStore API and UI components.

The project includes:

✔ API testing (user creation, authorization, book operations)

✔ UI exploratory testing

✔ Full bug documentation with screenshots

✔ Organized folder structure

✔ Clean and professional reporting

Project Structure
Web_Testing_Project/
│
├── README.md                     ← Main documentation (this file)
│
├── screenshots/                  ← API screenshots
│       └── readme.md             ← API screenshot index
│
└── screenshots-bugs/             ← UI bug screenshots
        └── readme.md             ← Bug descriptions


🔵 1. API Testing Overview

API under test: DemoQA BookStore API
https://demoqa.com/swagger/#/BookStore

Tested endpoints:

POST /Account/v1/User – create user

POST /Account/v1/GenerateToken – generate token

POST /Account/v1/Authorized – verify authorization

GET /BookStore/v1/Books – get all books

GET /BookStore/v1/Book – get book by ISBN

POST /BookStore/v1/Books – add books to collection

DELETE /BookStore/v1/Book – delete book

DELETE /BookStore/v1/Books – delete all user books

Negative tests: invalid password, invalid token, invalid ISBN

📸 All API screenshots are here:
➡ /screenshots

🔵 2. UI Testing Overview

Performed exploratory UI testing on:

WebTables

Slider

Selectable (List/Grid)

Menu

Radio Buttons

Resizable

Book Store Page

Found multiple reproducible visual and functional bugs.

📸 All bug screenshots with descriptions are here:
➡ /screenshots-bugs

🐞 3. Summary of Found UI Bugs

Here are some examples (full list in /screenshots-bugs/readme.md):

✔ Bug: WebTables loads empty

The table displays no records.

✔ Bug: Book page opens as white screen

Clicking on a book leads to blank page.

✔ Bug: “No” radio button not clickable

Element is disabled.

✔ Bug: Slider does not drag properly

Moves one step only, shows forbidden icon.

✔ Bug: Numbers in list/grid “stick” to cursor

Visual glitch while selecting.

✔ Bug: “More” button in Menu not working

No dropdown activation.

✔ Bug: Resizable box behaves inconsistently

Jerky movement, not smooth.

🧪 4. Skills Demonstrated
✔ Manual API testing

status codes

positive & negative cases

authorization

JSON body validation

✔ UI exploratory testing

visual bugs

interactive element testing

usability issues

✔ Bug reporting

clear STR (steps to reproduce)

expected vs actual result

attached evidence

✔ GitHub project structuring

folder structure

documentation

commit history

🏁 5. Final Notes

This project demonstrates my ability to:

analyze API behavior

identify UI problems

write clean bug reports

document everything professionally

organize QA work into a portfolio-ready project

💛 Author

Karina Kuzmina
Aspiring QA Engineer / Future Backend Developer

## ✔ Test Cases — BookStore API

### Test Case 1 — Create User (Positive)
| Field | Description |
|-------|-------------|
| **ID** | TC_API_001 |
| **Title** | Create new user with valid data |
| **Precondition** | No user with same username exists |
| **Steps** | 1. Send POST /Account/v1/User with valid body |
| **Expected Result** | 201 Created, userID returned |
| **Status** | Passed |

### Test Case 2 — Create User (Negative: weak password)
| Field | Description |
|-------|-------------|
| **ID** | TC_API_002 |
| **Title** | Create user with invalid password |
| **Steps** | 1. Send POST with password "123" |
| **Expected Result** | 400 Bad Request, password validation error |
| **Status** | Passed |

### Test Case 3 — Generate Token
| Field | Description |
|-------|-------------|
| **ID** | TC_API_003 |
| **Title** | Generate token with valid credentials |
| **Expected Result** | 200 OK, token string generated |

### Test Case 4 — Authorization Check
| Field | Description |
|-------|-------------|
| **ID** | TC_API_004 |
| **Title** | Check authorization with valid credentials |
| **Expected Result** | true |

### Test Case 5 — Add Book to Collection
| Field | Description |
|-------|-------------|
| **ID** | TC_API_005 |
| **Title** | Add book with valid ISBN |
| **Expected Result** | 201 Created |

### Test Case 6 — Delete Book
| Field | Description |
|-------|-------------|
| **ID** | TC_API_006 |
| **Title** | Delete book from user collection |
| **Expected Result** | 204 No Content |

## 🐞 Bug Tracking Table

| Bug ID | Title | Severity | Priority | Status |
|--------|--------|----------|----------|--------|
| B001 | WebTables loads empty | High | High | Open |
| B002 | Book details page is white screen | High | High | Open |
| B003 | Radio button “No” not clickable | Medium | Medium | Open |
| B004 | Slider moves incorrectly | Medium | Low | Open |
| B005 | Grid numbers stick to cursor | Low | Low | Open |
| B006 | List numbers stick to cursor | Low | Low | Open |
| B007 | “More” button inactive | Medium | Low | Open |
| B008 | Resizable box jumps / not smooth | Medium | Low | Open |

## ✔ UI Testing Checklist

### General UI
- [x] Page loads correctly
- [x] All text is readable
- [x] No broken elements
- [x] Buttons clickable
- [x] Hover states visible

### Interactive Elements
- [x] Slider movement
- [x] Resizable components
- [x] Radio buttons
- [x] List/Grid selection
- [x] Menu navigation

### BookStore UI
- [x] Book list loads
- [x] ISBN navigation works
- [ ] Book details page loads correctly (❌ Bug found)

# 📄 Additional QA Documentation

This project also includes:

### ✔ API Test Cases  
Located in the README (section: Test Cases).

### ✔ Bug Tracking Table  
All bugs tracked with severity and priority.

### ✔ UI Testing Checklist  
Covers general UI, interactive elements, and BookStore functionality.

Together, these documents demonstrate my ability to test APIs, analyze UI behavior, identify bugs, and structure QA work professionally.
