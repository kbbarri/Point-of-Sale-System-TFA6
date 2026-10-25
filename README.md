# Laravel POS System – TFA6

A simple Point of Sale (POS) application developed using Laravel 12. This project builds upon TFA5 by replacing static PHP arrays with a SQLite database and Eloquent models.

## Pages

- **Home** (`/`) – Landing page
- **About** (`/about`) – Information about the POS system
- **Customer Accounts** (`/customers`) – Displays customer records from the database
- **User Accounts** (`/users`) – Displays user records from the database

## Features

- Laravel routing and controllers
- Blade templates with `@foreach`
- SQLite database
- Customer and User Eloquent models
- Database migrations
- Database seeders with five sample records per table
- Navigation between four pages

## Technologies Used

- PHP
- Laravel 12
- SQLite
- Eloquent ORM
- Blade Templates
- HTML

## Database Structure

**Customers Table**
- `id`
- `full_name`
- `email`
- `phone`
- `created_at`

**Users Table**
- `id`
- `username` (unique)
- `full_name`
- `created_at`

## How to Run

1. Install PHP and Composer.
2. Clone or download the complete Laravel project.
3. Run `composer install`.
4. Copy `.env.example` to `.env`.
5. Set `DB_CONNECTION=sqlite` in `.env`.
6. Create an empty `database/database.sqlite` file if it doesn't exist.
7. Run `php artisan key:generate`.
8. Run `php artisan migrate:fresh --seed` on a new, empty development database.
9. Start the server using `php artisan serve`.
10. Open `http://127.0.0.1:8000`.

## Note

The application uses Eloquent models to retrieve customer and user records from the SQLite database instead of static PHP arrays.
