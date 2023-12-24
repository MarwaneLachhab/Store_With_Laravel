# Store_With_Laravel - Admin and User Sections

This project is a web store built using Laravel framework with separate sections for admins and users.

## Features

- **Admin Section:**
  - Manage products, categories, and orders
  - Dashboard for sales analytics
  - User management and permissions

- **User Section:**
  - Browse products by category
  - Add products to cart
  - Checkout functionality

## Prerequisites

- PHP (version 8.1 or newer)
- Composer
- phpMyAdmin

## Installation

1. **Clone the repository:**

   `git clone https://github.com/MarwaneLachhab/Store_With_Laravel.git`

2. **Navigate to the project directory:**

   `cd laravel-store`

3. **Install dependencies:**

   `composer install`

4. **Setup environment variables:**

   - Rename .env.example to .env
   - Configure your database credentials in the .env file

5. **Run migrations and seeders:**

   `php artisan migrate --seed`

6. **Generate application key:**

   `php artisan key:generate`

7. **Start the development server:**

   `php artisan serve`

   The application will be available at http://localhost:8000.
   
7. **Importing the SQL Database using phpMyAdmin
    Login to phpMyAdmin:

   Open your web browser and go to your phpMyAdmin URL.
   Log in using your credentials.
   Access Import:

   Select the database where you want to import data or create a new one.
    Go to the "Import" tab.
    Choose File:

    Click "Choose File" and select bd-pfe-2.sql from your computer.
    Configure Import:

    Verify character encoding and collation settings.
    Leave most settings as default.
    Start Import:

    Click "Go" or "Import" to begin the import process.
    Wait for Completion:

    It may take time depending on the file size. phpMyAdmin will display a message when done.
    Configuring Laravel to Use the Imported Database
    Update .env File:

    Open your Laravel project's .env file.
    Update Database Credentials:

    Update these lines with the correct details:
    makefile
    Copy code
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_database_name
    DB_USERNAME=your_database_username
    DB_PASSWORD=your_database_password
    Replace your_database_name, your_database_username, and your_database_password with the credentials for the imported database.

    Connect Laravel to the Database:

    Ensure Laravel is using the updated database credentials by applying these changes in your Laravel application's database configuration.
    After these steps, your Laravel application should be connected to the imported database, allowing you to utilize its data within your application.

    Remember to back up any existing databases before importing to avoid data loss and ensure the correctness of credentials in the .env file for proper database        connection.

## Usage

Accessing Admin Section
To access the admin functionalities:
- Use the following URL: [http://localhost:8000/login](http://localhost:8000/login)
- Log in using the provided admin credentials.
After logging in, you'll have access to the admin dashboard and functionalities for managing products, categories, orders, and user permissions.
- Explore the functionalities available for managing products, categories, and orders
Accessing user Section
To access the user functionalities:
- Switch to the user section with logout 
- Browse products, add them to cart, and proceed with the checkout process

## Admin Credentials

- Username: admin@gmail.com
- Password: 12345678

## Contributing

1. Fork the repository
2. Create a new branch (git checkout -b feature/new-feature)
3. Make your changes
4. Commit your changes (git commit -am 'Add new feature')
5. Push to the branch (git push origin feature/new-feature)
6. Create a pull request

## License

This project is licensed under the MIT License.
