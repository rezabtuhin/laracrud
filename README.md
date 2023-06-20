<p align="center"><img src="https://camo.githubusercontent.com/0d601c68ab4ee554491ffe2aa994f48e47ff6447f295e1a359a07fb9fb070a64/68747470733a2f2f332e62702e626c6f6773706f742e636f6d2f2d6a7779624b6a314d6e49552f57423676395448714b7a492f414141414141414149586b2f475030673553313643656f31505032353254325259704d674156684a6866544541434c63422f73313630302f435255442e706e67" width="400" alt="Laravel Logo"></p>

## About project

It's a simple API request/response `CRUD` application made with Laravel.

## Features

| Method | Name                 | API call       | Response                                    | Note                                   |
| ------ | -------------------- | -------------- | ------------------------------------------- | -------------------------------------- |
| POST   | User Registration    | api/register   | Success                                     | Require json body                      |
| POST   | Login                | api/login      | Authentication token                        | Require json body                      |
| POST   | Add product          | api/products   | Created product                             | Require authentication key & json body |
| GET    | Show all products    | api/products   | All products                                | Requires nothing                       |
| GET    | Get specific product | api/products/1 | Returns product of id 1 (if exists)         | Requires nothing                       |
| PUT    | Update product       | api/products/1 | Returns updated product of id 1 (if exists) | Require authentication key & json body |
| DELETE | Delete product       | api/products/1 | Delete product of id 1 (if exists)          | Require authentication key             |
| POST   | Logout               | api/logout     | Logout of the system                        | Require authentication key             |

## Accepted/Required json keys

**Registration:** `name`, `email`, `password`, `password_confirmation`<br>
**Login:** `email`, `password` <br>
**Add products:** `name`, `slug`, `description`, `price` <br>
**Update products:** `name`, `description`, `price` [Note: not all the field is required here]<br>

## Postman configuration

[Download](https://www.postman.com/downloads/) and install the Postman desktop application. Create a new collection then create a new global variable `token` for authorization. Initialize the variable with the token from the response of login. Now navigate to the API request window, search for `Authorization` tab; Select type `Bearer Token` and set the `token` in the Token field. **[NOTE: global variable `token` must be reinitialized with the new token value from the response of login every time after logout.]**

-   Set Headers to accept `application/json` and use `x-www-form-urlencoded` where needed for convenience.

## Installation

Your machine must have composer, php, xampp, git, node installed.

### Step 1: Clone the repository/Download ZIP

```sh
https://github.com/rezabtuhin/laracrud.git
```

### Step 2: Navigate to the project directory on your desktop.

### Step 3: Open the terminal and run these commands (Requires all commands).

```sh
composer install
```

```sh
npm install
```

```sh
cp .env.example .env
```

Set up the database in the `.env` file and your `MySQL` server and configurations. Then run-

```sh
php artisan key:generate
```

```sh
php artisan migrate
```

```sh
php artisan serve
```

Sample postman config file: [Download](https://drive.google.com/file/d/11YluTbeROaxTn17G0jJ8wUsHiu5DnU2y/view?usp=sharing) here.

<p align="center" style="font-weight: bold">Good luck 😃</p>
