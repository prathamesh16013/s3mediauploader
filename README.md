# s3mediauploader
first install nginx,php and mariadb and start the services

sudo yum install php-mysqlnd -y

go to default path of nginx and create .html and .php file
then installl:
sudo curl -sS https://getcomposer.org/installer | sudo php
sudo mv composer.phar /usr/local/bin/composer
sudo ln -s /usr/local/bin/composer /usr/bin/composer
sudo composer require aws/aws-sdk-php

then go to mysql and create the database and table.

create table users (id int primary key auto_increment, name varchar(100), surname varchar(100), gender varchar(100),email varchar(100), image_url varchar(100));

and restart the all services and host to the browser.
