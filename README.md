<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://camo.githubusercontent.com/0d601c68ab4ee554491ffe2aa994f48e47ff6447f295e1a359a07fb9fb070a64/68747470733a2f2f332e62702e626c6f6773706f742e636f6d2f2d6a7779624b6a314d6e49552f57423676395448714b7a492f414141414141414149586b2f475030673553313643656f31505032353254325259704d674156684a6866544541434c63422f73313630302f435255442e706e67" width="400" alt="Laravel Logo"></a></p>

## About project

It's a simple API request/response `CRUD` application made with Laravel.

## Features

| Method | Name                 | API call       | Response                                    | Note                                   |
| ------ | -------------------- | -------------- | ------------------------------------------- | -------------------------------------- |
| POST   | User Registration    | api/register   | Success                                     | Requie json body                       |
| POST   | Login                | api/login      | Authentication token                        | Requie json body                       |
| POST   | Add product          | api/products   | Created product                             | Require authentication key & json body |
| GET    | Show all products    | api/products   | All products                                | Requires nothing                       |
| GET    | Get specific product | api/products/1 | Returns product of id 1 (if exists)         | Requires nothing                       |
| PUT    | Update product       | api/products/1 | Returns updated product of id 1 (if exists) | Require authentication key & json body |
| DELETE | Delete product       | api/products/1 | Delete product of id 1 (if exists)          | Require authentication key             |
| POST   | Logout               | api/logout     | Logout of the system                        | Require authentication key             |

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

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
