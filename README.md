# cosc480final
Banking Application

This is a simple banking application that allows users to register, login, and perform transactions. It is built using Node.js, Express, and MySQL.
Installation

    Clone the repository:

    bash

git clone https://github.com/yourusername/banking-app.git

Install dependencies:

bash

cd banking-app
npm install

Set up the database:

    Create a MySQL database named bank_database.
    Update the MySQL connection details in script.js with your database credentials.

Start the application:

bash

    npm start

    Open your web browser and navigate to http://localhost:3001 to access the application.

Usage

    Register a new account by navigating to /register and filling out the registration form.

    Login with your registered credentials at /login.

    Perform transactions (withdrawals or deposits) at /transactions.

    View account details and transaction history at /display.

Files and Directories

    routes/auth.js: Contains routes for user registration, login, and transactions.
    routes/pages.js: Contains routes for rendering HTML pages.
    controller/auth.js: Contains controller functions for handling user registration.
    script.js: Main entry point of the application, sets up the server and routes.
    views/: Directory containing Handlebars (.hbs) templates for rendering pages.

Dependencies

    Express: Web framework for Node.js.
    MySQL2: MySQL client for Node.js.
    Express-session: Middleware for managing session data.
    Body-parser: Middleware for parsing request bodies.
    Handlebars: Templating engine for rendering views.
