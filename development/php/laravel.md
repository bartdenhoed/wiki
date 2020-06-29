# Knowledge Base - Development - Laravel

### JWT

Source code:
Docs: https://jwt-auth.readthedocs.io/en/docs/laravel-installation/

Article tutorial: https://medium.com/employbl/build-authentication-into-your-laravel-api-with-json-web-tokens-jwt-cd223ace8d1a
Article tutorial (2019): https://www.cloudways.com/blog/laravel-jwt-authentication/
YouTube tutorial: https://www.youtube.com/watch?v=l201RSQ7Ti4

Example project: https://github.com/ZanichelliEditore/laravel-jwt-idp




# Laravel - Documentation

- [Laravel - Documentation](#laravel---documentation)
    - [General Laravel](#general-laravel)
        - [Start new project](#start-new-project)
        - [Laracasts](#laracasts)
        - [Overige](#overige)
        - [Artisan](#artisan)
        - [Folder structure](#folder-structure)
        - [Migrations](#migrations)
        - [Eloquent](#eloquent)
        - [Routing](#routing)
        - [Telescope](#telescope)
        - [Repeating](#repeating)
    - [Methods](#methods)
        - [Generators](#generators)
    - [Debugging](#debugging)
        - [DumpDie](#dumpdie)
        - [Dump](#dump)
        - [Logger](#logger)
    - [Laravel 6](#laravel-6)
        - [Lazy Collections](#lazy-collections)
        - [Ignition](#ignition)
        - [Frondend Scaffolding](#frondend-scaffolding)
        - [Eloquent Subquery Additions](#eloquent-subquery-additions)
    - [NOTES:](#notes)

### General Laravel

##### Start new project
1. `laravel new [name]`
2. Edit `.env` file
3. Generate key `php artisan key:generate`

##### Laracasts
**Defenition**
- Started: 🕐
- Done: ✅

**Series:**
- [Laravel 5.7 From Scratch](https://laracasts.com/series/laravel-from-scratch-2018/) 
- [Laravel TDD Birdboard](https://laracasts.com/series/build-a-laravel-app-with-tdd) 🕐
- [Laravel Explained](https://laracasts.com/series/laravel-explained)
- [What's New in Laravel 5.8](https://laracasts.com/series/whats-new-in-laravel-5-8)
- [What's New in Laravel 6](https://laracasts.com/series/whats-new-in-laravel-6) ✅
- [Laravel 6 From Scratch](https://laracasts.com/series/laravel-6-from-scratch)

##### Overige
- [Server Admin for Programmers](https://serversforhackers.com/)
- [Laravel Spark](https://spark.laravel.com/)

##### Artisan
Use this CLI commando to create default files like:
- Webserver: `php artisan serve`
- CLI interface: `php artisan tinker`
- Helper: `php artisan help [action]`
>
- Generate key: `php artisan key:generate`
>
- Create controller: `php artisan make:controller [-r] [ControllerName] [-m] [Model]`
- Create migration: `php artisan make:migration [create_example_table]`
- Create model: `php artisan make:model [Name]`

##### Folder structure
[https://laravel.com/docs/5.8/structure](https://laravel.com/docs/5.8/structure)
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


##### Migrations
Database version control.

- `php artisan migrate` install
- `php artisan migrate:rollback`
- Drop all tables: `php artisan migrate:fresh`

##### Eloquent

##### Routing
Shorthand: `Route::resource('projects', 'ProjectsController');`

All methods:
- GET `/projects` -> index (all projects)
>
- GET `/projects/1` -> show (1 project)
- GET `/projects/create` -> create (create form)
- POST `/projects` -> store (insert project)
>
- GET `/projects/1/edit` -> edit (edit project)
- PATCH `/projects/1` -> update (update project)
>
- DELETE `/projects/1` -> destory (delete project)

##### Telescope
https://laravel.com/docs/5.8/telescope

##### Repeating
https://laracasts.com/series/laravel-from-scratch-2018/episodes/19
https://laracasts.com/series/laravel-from-scratch-2018/episodes/20
https://laracasts.com/series/laravel-from-scratch-2018/episodes/21
https://laracasts.com/series/laravel-from-scratch-2018/episodes/22

https://www.youtube.com/watch?v=l201RSQ7Ti4

### Methods

##### Generators
- [Laracasts](https://laracasts.com/series/laravel-explained/episodes/3)







### Debugging
##### DumpDie
- [Laravel](https://laravel.com/docs/master/helpers#method-dd)
```php
// TODO
dd();
```

##### Dump
- [Laravel](https://laravel.com/docs/master/helpers#method-dump)
```php
// TODO
dump();
```

##### Logger
- [Laravel](https://laravel.com/docs/master/logging)
```php
// Create file in logs/laravel-[date].log
logger($arrayOrObject);

// Get file
readFile(storage_path('logs/laravel-[date].log'));
```

### Laravel 6
- [GitHub](https://github.com/laravel/laravel)
- [Documentation](https://laravel.com/docs/6.x)
- [Laravel News](https://laravel-news.com/laravel-6)

##### Lazy Collections
Add Lazy Collections to fix memory issues:
- [Laracasts](https://laracasts.com/series/whats-new-in-laravel-6/episodes/1)
- [GitHub](https://github.com/laravel/framework/pull/29415)

**Example:** Fetch all projects with all collections:

```php
// Big query
$projects = \App\Project::all();
```

**Example:** With a generator only fetch the requested collections:

```php
// No query
$projects = \App\Project::cursor();

// Small query
$projects->first();
```

##### Ignition
Ignition: a new error page for Laravel:

- [Laracasts](https://laracasts.com/series/whats-new-in-laravel-6/episodes/2)
- [Introduction blog](https://freek.dev/1441-ignition-a-new-error-page-for-laravel)
- [GitHub](https://github.com/facade/ignition)
- [Config file](https://github.com/facade/ignition/blob/master/config/ignition.php)
    - Darkmode
    - Default editor
- [Ignition tinker tab](https://github.com/facade/ignition-tinker-tab)

##### Frondend Scaffolding
- [Laracasts](https://laracasts.com/series/whats-new-in-laravel-6/episodes/3)
```php
composer require laravel/ui
php artisan ui:auth
```

##### Eloquent Subquery Additions
- [Laracasts](https://laracasts.com/series/whats-new-in-laravel-6/episodes/4)


### NOTES:

Gedeelde code:
Channels?
Broadcast?
Packages?

Eigen packages voor meerder Laravel applicaties
