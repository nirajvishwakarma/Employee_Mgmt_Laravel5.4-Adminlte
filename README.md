## Available functionalities:

+ Login and logout, forget password  (Lock account in 5 minutes after 3 failed attempts).

+ Manage employees (Add, edit and delete).

+ Manage countries, cities, states (Add, edit and delete).

+ Manage users (Add, edit and delete).

+ Manage salary (Add, edit and delete).

+ Manage division (Add, edit and delete).

+ Manage departments (Add, edit and delete).

+ Make reports (export to Excel and PDF).

+ Search (with multiple combine fields).

+ Pagination

+ Validation

+ Responsive

## Guide Video
https://www.youtube.com/watch?v=Jbt5bEgv_QM

## LAMP Setup
https://www.tecmint.com/install-lamp-with-phpmyadmin-in-ubuntu-20-04/

## STEP to follow

apt update
sudo apt install apache2 -y

sudo systemctl start apache2
sudo systemctl enable apache2
sudo systemctl status apache2
sudo systemctl is-enabled apache2


sudo apt install mariadb-server mariadb-client -y

sudo systemctl start mariadb
sudo systemctl enable mariadb
sudo systemctl status mariadb
sudo systemctl is-enabled mariadb

sudo mysql_secure_installation


sudo apt install php libapache2-mod-php php-mysql -y


apt install composer
composer update

rename .env.example to .env
configure database in .env file

create a new database with name : employees_db
create a new table with : php artisan migrate
create a default user with system with : php artisan db:seed

php artisan key:generate
Execute: php artisan config:clear
Execute: php artisan serve --host 0.0.0.0

DONE


CREATE USER 'test'@'%' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGE ON *.* TO 'test'@'%';

## Hotfix Videos
https://www.youtube.com/watch?v=bDmmKOdgIeY

https://www.youtube.com/watch?v=cEdQvdYLuSg

## License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).

## ☕ Support

You can support me so that there will be more good open source projects in the future
<p align="center" style="padding: 10px 0 20px 0">
  <a href="https://www.buymeacoffee.com/hdcoder" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="50" width="220">
  </a>
</p>
