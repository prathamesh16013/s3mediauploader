# s3mediauploader

launch instance ,
create database using rds, 
create role in iam as a s3 full access and attach that role to ec2 instance, 
create ACL enabled S3 bucket
first install nginx ,php and mariadb and start the services in ec2 instance then install connector
sudo yum install php-mysqlnd -y for amazon linux or use 
sudo apt-get install php-mysqlnd -y for ubuntu
go to default path of nginx and create .html and .php file
then installl: SDK  for php

sudo curl -sS https://getcomposer.org/installer | sudo php
sudo mv composer.phar /usr/local/bin/composer
sudo ln -s /usr/local/bin/composer /usr/bin/composer
sudo composer require aws/aws-sdk-php

then go to mysql and create the database and table.

create table users (id int primary key auto_increment, name varchar(100), surname varchar(100), gender varchar(100),email varchar(100), image_url varchar(100));

and restart the all services and host to the browser.
