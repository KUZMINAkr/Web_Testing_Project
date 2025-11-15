🌐 Web & API Testing Project — DemoQA

By Karina Kuzmina

This project demonstrates manual API testing, UI functional testing, and bug reporting skills using DemoQA’s BookStore API and UI components.

The project includes:

✔ API testing (user creation, authorization, book operations)

✔ UI exploratory testing

✔ Full bug documentation with screenshots

✔ Organized folder structure

✔ Clean and professional reporting

📁 Project Structure
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
