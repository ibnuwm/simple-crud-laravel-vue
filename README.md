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

6. Create route api.php

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

### Frontend Vue

1. Install npm dependencies

```install-npm
npm install
npm install vue vue-router vue-axios vue-devtools
npm install vue bootstrap bootstrap-vue
1. npm run watch
2. php artisan serve
```

2. Edit resources/view/welcome.blade.php

```welcome
<html>

<head>
    <link href="{{ mix('css/app.css') }}" type="text/css" rel="stylesheet" />
    <script src="{{ mix('js/app.js') }}" type="text/javascript" defer></script>
</head>

<body style='background-color: white'>
    <div id="app">
    </div>
</body>

</html>
```

3. routes web.php

```route
Route::get('/{any}', function () {
    return view('welcome');
})->where('any','.*');
```

4. Configure vue router in resources/js/components

```vue router
App.vue : sebagai root/parent dari view. Create.vue : digunakan untuk form
tambah data Read.vue : digunakan untuk menampilkan semua data Update.vue :
digunakan untuk memperbarui data
```
