--------- COMMANDS ---------

RUN docker via docker compose -> docker-compose up -d server

RUN and rebuild docker compose -> docker-compose up -d --build server

RUN php artisan -> docker-compose up --rm artisan migrate(commads)

RUN composer -> docker-compose up --rm composer create-project laravel/laravel:^8.0 .

---

HOW TO USE

1. Create folder and name it as src
2. Edit env/mysql.env file for the database name, username, password and root password
3. Install laravel by using this command -> docker-compose up --rm composer create-project laravel/laravel:^8.0 .
4. Edit the .env file for laravel in /src/.env directory
5. Run the artisan to migrate the database -> hp artisan -> docker-compose up --rm artisan migrate
6. Run the container in order to lunch the application -> docker-compose up -d --build server

to access phpyadmin:
localhost:3000
