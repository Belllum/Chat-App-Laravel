# Real-Time Chat System

A real-time chat application built using Laravel (with Reverb) for the backend and React for the frontend.

## Features

-   Real-time messaging
-   User authentication (register/login)
-   Single chat channel for all users

## Installation

### Prerequisites

-   Node.js
-   Composer
-   PHP
-   MySQL
-   Git

### Setup

1. Install dependencies:

    ```bash
    composer install
    ```

2. Copy the `.env.example` file to `.env`:

    ```bash
    cp .env.example .env
    ```

3. Configure your `.env` file:

    ```env

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_database
    DB_USERNAME=your_username
    DB_PASSWORD=your_password

    ```

4. Run migrations:

    ```bash
    php artisan migrate
    ```

## Running the App

After setting up the app, open four(4) terminals and run the following commands in your project directory:

```bash
php artisan serve
php artisan queue:listen
php artisan reverb:start
npm run dev

```

## Technologies Used

-   **Frontend**: React
-   **Backend**: Laravel (with Reverb), MySQL
