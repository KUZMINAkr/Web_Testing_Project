📘 BookStore API Testing Documentation
1. Overview

This document contains the results of manual API testing performed on DemoQA BookStore API.
Requests were executed with authorization, and all endpoints were checked for correct logic, status codes, and responses.

2. Tested Endpoints

POST /Account/v1/User — Create user

POST /Account/v1/GenerateToken — Generate token

POST /Account/v1/Authorized — Check authorization

POST /BookStore/v1/Books — Add books to user

DELETE /BookStore/v1/Book — Delete one book

DELETE /BookStore/v1/Books — Delete all user books

3. Test Flows
### 3.1 Create User

POST /Account/v1/User

Example request:

{
  "userName": "minimi3433",
  "password": "Qwerty124324!"
}


Expected:

201 Created

userID is not empty

books: []

📎 Screenshot:
![Create User](screenshots/user.png)

3.2 Generate Token

POST /Account/v1/GenerateToken

Example request:

{
  "userName": "minimi3433",
  "password": "Qwerty124324!"
}


Expected:

200 OK

"token" is generated

"status": "Success"

"result": "User authorized successfully."

📎 Screenshot:
![Token](screenshots/tocken.png)

3.3 Authorization Check

POST /Account/v1/Authorized

Example request:

{
  "userName": "minimi3433",
  "password": "Qwerty124324!"
}


Expected:

200 OK

Response: true

📎 Screenshot:
![Authorized](screenshots/true.png)

3.4 Add Books to User

POST /BookStore/v1/Books

Example request:

{
  "userId": "58eb34ae-dc42-4123-89ab-10d63ebc800f",
  "collectionOfIsbns": [{
    "isbn": "9781449325862"
  }]
}


Expected:

201 Created

The book should appear in user profile

📎 Screenshot:
![Add Books](screenshots/bookstore.png)

3.5 Delete a Book

DELETE /BookStore/v1/Book

Example request:

{
  "isbn": "9781449325862",
  "userId": "58eb34ae-dc42-4123-89ab-10d63ebc800f"
}


Expected:

204 No Content

📎 Screenshot:
![Delete Book](screenshots/delete.png)

3.6 Invalid Password Error

Example request:

{
  "userName": "minimi3433",
  "password": "123"
}


Expected:

400 Bad Request

"message": "Password must contain at least..."

📎 Screenshot:
![Password Error](screenshots/password must be.png)

3.7 Get Book by ISBN (UI behavior check)

Opening:

https://demoqa.com/books?book=9781449325862


Expected:

Page should load book details

Actual:

White blank screen

📎 Screenshot:
![ISBN Issue](screenshots/ISBN.png)

✔️ API Testing Completed Successfully
