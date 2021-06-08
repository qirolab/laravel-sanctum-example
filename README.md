# Laravel Sanctum Example

Watch tutorial: **[SPA Authentication using Vue.js And Laravel Sanctum](https://www.youtube.com/watch?v=8Uwn5M6WTe0)**.

## Common Errors

### 401 Errors

If you recieve a 401 error after registering and logging in you may need to add the following to your .env file.

```
SESSION_DRIVER=cookie
SESSION_LIFETIME=120
SESSION_DOMAIN=localhost
SANCTUM_STATEFUL_DOMAINS=localhost:8080
```

### CORS Errors

Recieving a CORS error is typically if your vue app can't communicate with your backend (Laravel). Make sure that the project is running. 
You can execute the following command to start the php server.

```
php artisan serve
```

## Laravel setup

### Install composer dependencies

```
cd laravel-sanctum
composer install
```

### Database Migrations

After installing composer dependencies, add your database credentials in `.env` file and then run migrations.

```
php artisan migrate
```

Now, in the terminal run `artisan serve` command. It will run the application at `http://127.0.0.1:8000` URL, and that URL path used in the Vue.js app.

```
php artisan serve
```

If you are running the Laravel API on a different URL path, then you need to update the URL path in the `src/apis/Api.js` of the Vue.js app.

## Vue.js Project setup

```
cd vue-app
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```
