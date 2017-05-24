# Laravel
Laravel

Install git
https://git-scm.com/downloads
git --version

Clone project
git clone https://github.com/heroku/php-getting-started.git
cd php-getting-started

Install Heroku CLI
https://devcenter.heroku.com/articles/getting-started-with-php#set-up
heroku login
heroku git:remote -a [heroku-app-name]
git push heroku master
https://[heroku-app-name].herokuapp.com/

Install Composer
https://getcomposer.org/Composer-Setup.exe
composer -V
composer global require laravel/installer

Create new project
laravel new [project_name]
cd [project_name]

Setup PHP
http://windows.php.net/downloads/releases/php-7.1.5-Win32-VC14-x64.zip
php -v

Start server local http://127.0.0.1:8000
php artisan serve

Create Model
php artisan help make:model
php artisan make:model -m [ProjectModel]

Migration DB
php artisan migrate
php artisan migrate:rollback

Setup DB
https://cdn.mysql.com//Downloads/MySQLInstaller/mysql-installer-web-community-5.7.18.1.msi
mysql -u root -p
create database [project-db-name]
exit

Config connect DB
.env
