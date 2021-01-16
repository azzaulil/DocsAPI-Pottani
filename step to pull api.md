# Step to Pull Backend Develop

* open cmd at project laravel
* run `git pull origin develop`
* run `php artisan serve` to deploy

* Apabila ada update database,
    * run `php artisan migrate:fresh --seed`
    * run `php artisan passport:install` to create token user
