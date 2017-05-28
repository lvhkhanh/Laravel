# Laravel
Laravel

How to write this file
https://www.udacity.com/course/writing-readmes--ud777

Install git
https://git-scm.com/downloads
```
git --version
```

Using Git
```
git init

git status

git add [file_name]

git add -A .

git reset

git commit -m "msg"

git log --summary

git remote add origin [remoteUrl]

git push -u origin master

git pull origin master

git stash

git stash apply

git diff HEAD

git diff --staged

git checkout --

git branch

git checkout -b new_branch

git branch new_branch git checkout new_branch

git rm -r folder_of_cats

git commit -am

git merge

git branch -d --force (-f) -D
```

Clone project
```
git clone https://github.com/heroku/php-getting-started.git
cd php-getting-started
```

Install Heroku CLI
https://devcenter.heroku.com/articles/getting-started-with-php#set-up
https://devcenter.heroku.com/articles/getting-started-with-laravel
```
heroku login
heroku git:remote -a [heroku-app-name]
git push heroku master
```
you can open the website as follows:
```
heroku open
```
https://<heroku-app-name>.herokuapp.com/
Ensure that at least one instance of the app is running:
```
heroku ps:scale web=1
```
Check log:
```
heroku logs --tail
```

Setup PHP
http://windows.php.net/downloads/releases/php-7.1.5-Win32-VC14-x64.zip
```
php -v
cp php.ini-develpoment php.ini
```

Install Composer
https://getcomposer.org/Composer-Setup.exe
```
composer -V
```

Install Laravel
```
composer global require laravel/installer
composer update
```

Create new project
```
laravel new <project_name>
cd <project_name>
```
Start server local http://127.0.0.1:8000
```
php artisan serve
```

Create Model
```
php artisan help make:model
php artisan make:model -m <ProjectModel>
```

Migration DB
```
php artisan migrate
php artisan migrate:rollback
```

Setup DB
https://cdn.mysql.com//Downloads/MySQLInstaller/mysql-installer-web-community-5.7.18.1.msi
```
mysql -u root -p
create database <dbname>
exit
```

Config connect DB
```
.env
```

```
php artisan help make:controller
php artisan make:controller -m <Model> <Model>Controller
```

Route
```
Route::get('/', '<Model>Controller@index');
Route::resource('<model>s', '<Model>Controller');
php artisan route:list
```

