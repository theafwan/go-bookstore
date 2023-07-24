# Go Book Management System
This is a simple Go project that demonstrates how to use MySQL as a database in Golang, GORM for ORM, JSON marshaling/unmarshaling, project structure, and Gorilla Mux for routing.

### Features
* Add a book to the database
* Get a list of all books
* Get a single book by ID
* Update book details
* Delete a book from the database

### Prerequisites
Make sure you have the following installed:

* Go programming language (version 1.16+)
* MySQL database

### Setup
1.  Clone the repository:
    * git clone https://github.com/theafwan/go-bookstore.git
    * cd go-bookstore

2. Set up the database:

    * Create a new MySQL database and note down the database credentials (username, password, and database name).
    * Update the database connection details in the config/config.go file.

3. Install dependencies:

4. Run the application:
    * go run main.go

The application will start, and you can access it at http://localhost:8080.

### API Endpoints
* POST /api/book - Add a new book
* GET /api/book - Get a list of all books
* GET /api/book/{id} - Get a single book by ID
* PUT /api/book/{id} - Update book details
* DELETE /api/book/{id} - Delete a book

### Project Structure
The project follows the following directory structure:
.
│── pkg   
        ├── config
│           └── app.go
        ├── controllers
│           └── book-controller.go
        ├── models
│           └── book.go
        ├── routes
│           └── bookstore-routes.go
        ├── utils
│           └── utils.go
│── cmd
│       └── main.go
├── go.mod
├── go.sum
└── README.md

* config: Contains configuration files for the database and other settings.
* controllers: Defines the application's controllers, handling different HTTP endpoints.
* models: Contains the data models and database interactions.
* routes: Defines the API routes and uses Gorilla Mux for routing.
* utils: Contains utility functions used in the application.

### Dependencies
The project uses the following external dependencies:

* GORM: An ORM library for Golang, used for interacting with the MySQL database.
* Gorilla Mux: A powerful URL router and dispatcher for matching incoming requests to their respective handler functions.

### Contributions
Contributions to improve the project are welcome! Feel free to submit pull requests or open issues if you find any bugs or have suggestions for enhancements.