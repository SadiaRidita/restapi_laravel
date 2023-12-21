# Laravel REST API

This repository contains a simple REST API built using Laravel, following the concepts learned from a YouTube tutorial.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Authentication](#authentication)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project provides a foundation for building and extending a fully functional API using Laravel.

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/SadiaRidita/restapi_laravel.git
    ```

2. **Install dependencies:**

    ```bash
    composer install
    ```

3. **Copy the `.env.example` file to `.env` and configure your database connection:**

    ```bash
    cp .env.example .env
    ```

    Update the following section in the `.env` file with your database details:

    ```dotenv
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_database_name
    DB_USERNAME=your_database_username
    DB_PASSWORD=your_database_password
    ```

4. **Run migrations and seed the database:**

    ```bash
    php artisan migrate --seed
    ```

5. **Generate the application key:**

    ```bash
    php artisan key:generate
    ```

6. **Start the development server:**

    ```bash
    php artisan serve
    ```

## Usage

The API is now accessible at `http://localhost:8000`. You can use tools like [Postman](https://www.postman.com/) to interact with the API.

## Endpoints

Document your API endpoints here. Include information about available routes, request methods, and expected responses. For example:

- `GET /api/users`: Get a list of all users.
- `POST /api/users`: Create a new user.
- `GET /api/users/{id}`: Get details of a specific user.
- ...

## Authentication

If your API requires authentication, provide details on how to authenticate requests. Include information about API keys, tokens, or any other authentication mechanism.

## Testing

To run tests, use the following command:

```bash
php artisan test
