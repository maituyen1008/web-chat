# Realtime chat app using Laravel, VueJS, Redis, Laravel Echo Server

# Install Instruction
## Prerequisite
Please make sure you have `redis` on your PC first. Run `redis-cli` in command line to check whether you have `redis`

## Installation:
- Clone this project

Run following command on root folder:

	- composer install
	- npm install
	- npm install -g laravel-echo-server
	- cp .env.example .env
	- change LARAVEL_ECHO_SERVER_REDIS_HOST in `.env` from `redis` to `localhost`
	- php artisan key:generate

Open `resources/js/bootstrap.js` scroll to bottom and choose which host match to yours (`production` or `development`)

Then open your `.env` file and change database connection info as installed on your PC

Turn on Xampp, Access PHPMyadmin and create a database with the name you defined in `.env`

Run following command: 

	- php artisan migrate
	- php artisan serve
	- npm run watch (open in another terminal tab)
	- php artisan queue:work (open in another terminal tab)
	- laravel-echo-server start (open in another terminal tab)

Open browser in Chrome and another tab using incognito or other browser type (Safari, Firefox). Create an account and test your app.

Then you're ready to go
