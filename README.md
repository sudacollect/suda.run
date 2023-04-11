## Laravel suda

Install steps

#1 install laravel
```
composer create-project laravel/laravel example-app

cd example-app
```

#2 install suda
```
composer require gtdxyz/suda
```

#3 config database

```
#========= edit .env =========
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your-database
DB_USERNAME=your-database-user
DB_PASSWORD=your-database-pass

```

#4 install

```
php artisan suda:install
```