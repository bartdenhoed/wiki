# Wiki - Development - Laravel

### JWT

Source code:
Docs: https://jwt-auth.readthedocs.io/en/docs/laravel-installation/

Article tutorial: https://medium.com/employbl/build-authentication-into-your-laravel-api-with-json-web-tokens-jwt-cd223ace8d1a
Article tutorial (2019): https://www.cloudways.com/blog/laravel-jwt-authentication/
YouTube tutorial: https://www.youtube.com/watch?v=l201RSQ7Ti4

Example project: https://github.com/ZanichelliEditore/laravel-jwt-idp



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
