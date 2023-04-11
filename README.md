## Laravel suda

Install steps

###1 Laravel
```
composer create-project laravel/laravel example-app

cd example-app
```

###2 Suda
```
composer require gtdxyz/suda
```

###3 Database

```
// edit .env

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your-database
DB_USERNAME=your-database-user
DB_PASSWORD=your-database-pass

```

###4 Install

```
php artisan suda:install
```

###5 Auth

```
// edit config/auth.php

// add to guards
'operate' => [
    'driver'    => 'session',
    'provider'  => 'operates',
],

// add to providers
'operates' => [
    'driver' => 'authsuda_provider',
    'model' => Gtd\Suda\Models\Operate::class,
],
```

###6 open your-domain/admin

```
admin@suda.run
suda#2021
```