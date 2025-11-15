🌐 Web & API Testing Project — DemoQA

By Karina Kuzmina

This project demonstrates manual API testing, UI functional testing, and bug reporting skills using DemoQA’s BookStore API and UI components.

📁 Project Structure
Web_Testing_Project/
│
├── README.md                     ← Main documentation  
│
├── screenshots/                  ← API testing screenshots  
│       └── readme.md            
│
└── screenshots-bugs/             ← UI bug screenshots  
        └── readme.md

🔵 1. API Testing Overview

API under test: DemoQA BookStore API
https://demoqa.com/swagger/#/BookStore

Tested endpoints:

POST /Account/v1/User – create user

POST /Account/v1/GenerateToken – generate JWT token

POST /Account/v1/Authorized – verify authorization

GET /BookStore/v1/Books – retrieve all books

GET /BookStore/v1/Book – retrieve book by ISBN

POST /BookStore/v1/Books – add book to user collection

DELETE /BookStore/v1/Book – delete user book

DELETE /BookStore/v1/Books – clear user collection

✔ Positive & negative testing
✔ Status code validation
✔ JSON body validation

📸 All API screenshots are stored here:
➡ /screenshots

🔵 2. UI Testing Overview

Performed exploratory UI testing on:

WebTables

Slider

Selectable (List & Grid)

Menu

Radio Buttons

Resizable

BookStore UI

Found multiple UI/UX defects and visual inconsistencies.

📸 Full bug list with screenshots:
➡ /screenshots-bugs

🐞 3. Summary of Found UI Bugs

Below are some examples (full list in /screenshots-bugs/readme.md):

✔ B001 — WebTables loads empty

Table displays no data on initial load.

✔ B002 — Book details page opens blank

Clicking a book opens a white page with no content.

✔ B003 — “No” radio button is not clickable

Disabled unexpectedly.

✔ B004 — Slider moves incorrectly

Jumps instead of sliding, cursor shows “forbidden”.

✔ B005 — Selectable (Grid) numbers stick to cursor

Visual highlight remains after movement.

✔ B006 — Selectable (List) highlight broken

Style remains after deselection.

✔ B007 — “More” menu button inactive

No dropdown opens.

✔ B008 — Resizable block jumps

Not smooth, inconsistent size behavior.

🧪 4. Skills Demonstrated
✔ API Testing

Working with REST endpoints

Positive & negative test design

Authorization & authentication

Status code validation

JSON response analysis

✔ UI Testing

Exploratory testing

Checking interactive widgets

Visual issues & layout problems

Cross-element interaction

✔ Bug Reporting

Clear STR (Steps to Reproduce)

Expected vs Actual

Screenshots included

Severity & Priority assigned

✔ Documentation & Git

Structured project layout

Detailed README.md

Clean commits

Professional presentation of QA work

🏁 5. Final Notes

This project demonstrates my ability to:

analyze API behavior

identify UI issues

create structured test cases

write clean bug reports

document work professionally

prepare QA work for a portfolio

💛 Author

Karina Kuzmina
Aspiring QA Engineer / Future Backend Developer

✔ Test Cases — BookStore API
TC_API_001 — Create User (Positive)
Field	Description
Title	Create user with valid data
Precondition	Username does not exist
Steps	Send POST /User with valid body
Expected Result	201 Created, userID returned
TC_API_002 — Create User (Negative: weak password)
Field	Description
Steps	Send POST with password "123"
Expected Result	400 Bad Request — password validation error
TC_API_003 — Generate Token

| Expected Result | 200 OK, token generated |

TC_API_004 — Authorization Check

| Expected Result | Response: "result": true |

TC_API_005 — Add Book to Collection

| Expected Result | 201 Created |

TC_API_006 — Delete Book

| Expected Result | 204 No Content |

🐞 Bug Tracking Table
Bug ID	Title	Severity	Priority	Status
B001	WebTables loads empty	High	High	Open
B002	Book page is white screen	High	High	Open
B003	Radio button “No” disabled	Medium	Medium	Open
B004	Slider drag incorrect	Medium	Low	Open
B005	Grid items stick to cursor	Low	Low	Open
B006	List items stick to cursor	Low	Low	Open
B007	“More” menu inactive	Medium	Low	Open
B008	Resizable box jumps	Medium	Low	Open
✔ UI Testing Checklist
General UI

 Page loads correctly

 Text readable

 No broken elements

 Buttons clickable

 Hover states visible

Interactive Elements

 Slider

 Resizable

 Radio buttons

 List/Grid selections

 Menu buttons

BookStore

 Book list loads

 ISBN links work

 Book details page loads correctly (❌ Bug found)

📄 Additional QA Documentation

This project includes:

✔ API Test Cases

(included in README)

✔ Bug Tracking Table

(with severity + priority)

✔ UI Testing Checklist

(covers usability & interactive elements)

These documents together demonstrate structured, professional QA work suitable for a junior portfolio.

# 👩‍💻 Author  
**Karina Kuzmina**  
Aspiring QA Engineer | Future Backend Developer  
