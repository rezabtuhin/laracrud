<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://camo.githubusercontent.com/0d601c68ab4ee554491ffe2aa994f48e47ff6447f295e1a359a07fb9fb070a64/68747470733a2f2f332e62702e626c6f6773706f742e636f6d2f2d6a7779624b6a314d6e49552f57423676395448714b7a492f414141414141414149586b2f475030673553313643656f31505032353254325259704d674156684a6866544541434c63422f73313630302f435255442e706e67" width="400" alt="Laravel Logo"></a></p>

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

[Download](https://www.postman.com/downloads/) and install the postman desktop application. Create a new collections then create a new global variable `token` for authorization. Initialize the variable with the token from the response of login. Now navigate to the api request window, search for `Authorization` tab; Select type `Bearer Token` and set the `token` in the Token field. **[NOTE: global variable `token` must be reinitialize with new token value from the response of login everytime after logout.]**

-   Set Headers accept `application/json` and use `x-www-form-urlencoded` where needer for the convienience.

### Premium Partners

-   **[Vehikl](https://vehikl.com/)**
-   **[Tighten Co.](https://tighten.co)**
-   **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
-   **[64 Robots](https://64robots.com)**
-   **[Cubet Techno Labs](https://cubettech.com)**
-   **[Cyber-Duck](https://cyber-duck.co.uk)**
-   **[Many](https://www.many.co.uk)**
-   **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
-   **[DevSquad](https://devsquad.com)**
-   **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
-   **[OP.GG](https://op.gg)**
-   **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
-   **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
