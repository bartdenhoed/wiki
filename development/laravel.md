# Wiki - Development - Laravel

![development laravel](https://github.com/bartdenhoed/wiki/blob/master/.images/development_laravel.svg)

## Introduction


## Table of contents
* [General documentation](#general-documentation)
* [Artisan](#artisan)
* [Tutorials](#tutorials)

## General documentation
#### Directoy Structure
* [Directory Structure](https://laravel.com/docs/master/structure)
```
.
+-- app
|   +-- Http
|   |   +-- Controllers
|   |   |   +-- Controller.php
|   |   +-- Middleware
|   |       +-- VerifyCsrfToken.php
|   +-- [Model].php
|
+-- database
|   +-- migrations
|       +-- date_filename.php
|
+-- public
|   +-- css
|   |   +-- app.css
|   +-- js
|   |   +-- app.js
|   +-- index.php
|
+-- recourses
|   +-- js
|   +-- sass
|   +-- views
|       +-- welcome.blade.php
|
+-- routes
|   +-- web.php
```

#### Starting
1. Create new project `laravel new [projectname]`
2. Edit the `.env.` file

#### Routing
CRUD
* GET `/projects` -> index (all projects)
>
* GET `/projects/1` -> show (1 project)
* GET `/projects/create` -> create (create form)
* POST `/projects` -> store (insert project)
>
* GET `/projects/1/edit` -> edit (edit project)
* PATCH `/projects/1` -> update (update project)
>
* DELETE `/projects/1` -> destory (delete project)

## Artisan
* Create controller: `php artisan make:controller [-r] [ControllerName] [-m] [Model]`
* Create migration: `php artisan make:migration [create_example_table]`
* Create model: `php artisan make:model [Name]`
* Maintenance Mode: `php artisan down`
#### Tinker
* `php artisan tinker`
#### Migrations
Database version control.

* `php artisan migrate` install
* `php artisan migrate:rollback`
* Drop all tables: `php artisan migrate:fresh`

## Tutorials

#### [Laracasts](https://laracasts.com)
* [Laravel 6 From Scratch](https://laracasts.com/series/laravel-6-from-scratch) ✅
* [What's New in Laravel 7](https://laracasts.com/series/whats-new-in-laravel-7) ⌛
* [What's New in Laravel 8](https://laracasts.com/series/whats-new-in-laravel-8) ⌛
* [Static Site Generators](https://laracasts.com/series/static-site-generators) 🕐
* [Learn Telescope](https://laracasts.com/series/learn-telescope) 🕐
* [Build a Laravel App With TDD](https://laracasts.com/series/build-a-laravel-app-with-tdd) ⌛
* [Build a Staging Server](https://laracasts.com/series/build-and-configure-a-staging-server) 🕐

**Defenition**
* Todo: 🕐
* Doing: ⌛
* Done: ✅

#### Samples
* https://github.com/jivanrij/laravel-samples