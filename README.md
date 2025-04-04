
# Bookstore API

This is a simple RESTful API using GOLANG for managing a bookstore. It allows you to perform CRUD operations on books, such as creating, reading, updating, and deleting book records.

## Features

- Add a new book
- Retrieve all books
- Retrieve a book by ID
- Update a book's details
- Delete a book

## Project Structure
Bookstore_GO/
├── cmd/
│   └── main/
│       └── main.go              # Entry point of the application
├── pkg/
│   ├── config/
│   │   └── app.go               # Database connection setup
│   ├── controllers/
│   │   └── book-controller.go   # Handlers for book-related API endpoints
│   ├── models/
│   │   └── book.go              # Book model and database operations
│   ├── routes/
│   │   └── bookstore-routes.go  # API route definitions
│   └── utils/
│       └── utils.go             # Utility functions
├── .gitignore
├── go.mod
├── go.sum
└── README.md


## Installation

Set Up the MySQL Database
	1.	Create a database named simplerest.
	2.	Update the MySQL username, password, and database name in pkg/config/app.go in the Connect function.

Run the Application

Start the application using the following command:

go run cmd/main/main.go

The API will be accessible at:

http://localhost:9010

API Endpoints

| Method | Endpoint               | Description                      |
|--------|------------------------|----------------------------------|
| POST   | `/book/`                | Add a new book                   |
| GET    | `/book/`                | Get all books                    |
| GET    | `/book/{bookId}`        | Get a book by ID                 |
| PUT    | `/book/{bookId}`        | Update a book by ID              |
| DELETE | `/book/{bookId}`        | Delete a book by ID              |


