# SIMPLE CRUD LARAVEL VUE

## About Project

This project is about create simple CRUD using laravel as backend and vue.js as front end.

### Backend Laravel

1. Install Laravel

```install-laravel
composer create-project --prefer-dist laravel/laravel simple-crud-laravel-vue
```

2. Config Database

```config-db
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravelvue
DB_USERNAME=root
DB_PASSWORD=
```

3. Create table migration

```table-migration
php artisan make:migration create_persons_table
php artisan migrate
```

4. Create model

```model
php artisan make:model Person
```

5. Create controller

```controller
php artisan make:controller PersonController
```

6. Create route

```route
GET: /api/person
GET: /api/person/{id}
POST: /api/person
PUT: /api/person{id}
DELETE: /api/person/{id}
```

7. Run and testing

```run
php artisan serve
```
