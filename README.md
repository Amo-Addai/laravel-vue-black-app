# [Laravel Vue Black Dashboard](#)
<!-- (https://laravel-vue-black-app.AUTO.com/?ref=vbl-readme) -->

Full-stack platform, with a **Php - Laravel** Backend API, and a **Vue - Black** Frontend Dashboard app. Comes with a flexible architecture across a variety of devices, operating systems, and databases. 

Clone the repo  

```bash
$ git clone https://github.com/Amo-Addai/laravel-vue-black-app.git
$ cd laravel-vue-black-app
```

# Laravel API Setup

## Introduction

JSON:API is a specification for how a client should request that resources be fetched or modified, and how a server should respond to those requests. It is designed to minimize both the number of requests and the amount of data transmitted between clients and servers. This efficiency is achieved without compromising readability, flexibility, or discoverability.

[Click here to go to the JSON:API docs](https://explore.postman.com/api/6357/laravel-jsonapi)

## Prerequisites

### JSON:API backend
The Laravel JSON:API backend project requires a proper multi-threaded web server such as Apache/Nginx environment with PHP, Composer and MySQL.

**Do not use `php artisan serve` as it will result in stalled requests due to the single-threaded nature of the built-in PHP web server.** 

We strongly recommend using [Laradock](https://laradock.io/) for Linux and Mac or [Laragon](https://laragon.org/download/) for Windows if possible.

Other options for your local environment:
- Windows: [How to install WAMP on Windows](https://updivision.com/blog/post/beginner-s-guide-to-setting-up-your-local-development-environment-on-windows)
- Linux: [How to install LAMP on Linux](https://howtoubuntu.org/how-to-install-lamp-on-ubuntu)
- Mac: [How to install MAMP on MAC](https://wpshout.com/quick-guides/how-to-install-mamp-on-your-mac/)

You will also need to install Composer 2: [https://getcomposer.org/doc/00-intro.md](https://getcomposer.org/doc/00-intro.md)


### Vue Black frontend
The Vue Black frontend project requires a working local environment with NodeJS version 8.9 or above (8.11.0+ recommended), npm, VueCLI.

Install Node: https://nodejs.org/ (version 8.11.0+ recommended)

Install NPM: https://www.npmjs.com/get-npm

Install VueCLI: https://cli.vuejs.org/guide/installation.html

## Laravel JSON:API Project Installation

1. Navigate in your Laravel API project folder: `cd your-laravel-json-api-project`
2. Install project dependencies: `composer install`
3. Create a new .env file: `cp .env.example .env`
3. Add your own database credentials in the .env file in DB_DATABASE, DB_USERNAME, DB_PASSWORD
5. Create users table: `php artisan migrate --seed`
6. Generate application key: `php artisan key:generate`
7. Install Laravel Passport: `php artisan passport:install` and set in the .env file the CLIENT_ID and CLIENT_SECRET that you receive
8. Add your own mailtrap.io credentials in MAIL_USERNAME and MAIL_PASSWORD in the .env file

## Vue Black Dashboard Project Installation

1. Navigate to your Vue Dashboard project folder:  `cd your-vue-black-app-project`
2. Install project dependencies: `npm install`
3. Create a new .env file: `cp .env.example .env`
4. `VUE_APP_BASE_URL` should contain the URL of your Vue Black Dashboard Project (eg. http://localhost:8080/)
5. `VUE_APP_API_BASE_URL` should contain the URL of your Laravel JSON:API Project. (eg. http://localhost:3000/api/v1)
6. Run `npm run dev` to start the application in a local development environment or `npm run build`  to build release distributables.

