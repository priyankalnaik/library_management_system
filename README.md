# Library Book Management App

This is a web application built with ReactJS and NodeJS that allows you to manage books in a library. You can issue, return, and view the current books available in the library. The application uses a MySQL database for storing information about books, students, and book borrowing.

## Installation

To run this project on your local machine, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone repo_url
   ```

2. Navigate to the project directory in your terminal:

   ```bash
   cd library-book-management
   ```

3. Install dependencies for the frontend by navigating to the `frontend` directory and running:

   ```bash
   cd frontend
   npm install
   ```

4. Install dependencies for the backend by navigating to the `backend` directory and running:

   ```bash
   cd backend
   npm install
   ```

5. Make sure you have XAMPP installed and running to provide the MySQL database server.

6. Configure database credentials in the `backend/utilities/credentials.js` file according to your XAMPP setup.

## Database Setup

The project is designed to create the necessary database and tables automatically. Follow these steps to set up the database:

1. Start your XAMPP server.

2. Run the application to create the database and tables by executing the following command from the `backend` directory:

   ```bash
   npm run createDB
   ```

3. The database named `library` will be created along with the tables: `book`, `student`, and `borrow`.

4. You need to insert the initial data for students and books directly into the tables.

## Running the Application

To start the application, run the following command from the root directory:

```bash
npm run dev
```

This command uses the `concurrently` package to run both the frontend and backend servers simultaneously.

## Features

- **Books**: View a list of all the books available in the library.
- **Issue**: Issue a book to a student.
- **Return**: List books issued by a student and provide an option to return them.
- **Search**: Find students who have issued a particular book.
- **Navigation**: Easy navigation with the navbar component.


