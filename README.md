# s3mediauploader

launch instance ,
create database using rds, 
create role in iam as a s3 full access and attach that role to ec2 instance, 
create ACL enabled S3 bucket
first install nginx ,php and mariadb and start the services in ec2 instance then install connector
sudo yum install php-mysqlnd -y 
go to default path of nginx and create .html and .php file
then installl: SDK  for php

sudo curl -sS https://getcomposer.org/installer | sudo php
sudo mv composer.phar /usr/local/bin/composer
sudo ln -s /usr/local/bin/composer /usr/bin/composer
sudo composer require aws/aws-sdk-php

then go to mysql and create the database and table.

create table users (id int primary key auto_increment, name varchar(100), surname varchar(100), gender varchar(100),email varchar(100), image_url varchar(100));

and restart the all services and host to the browser.


stepwise Commands
     sudo apt update
     sudo yum update
     sudo yum install nginx php php-fpm php8.3-fpm -y
     sudo service nginx start
     sudo service php-fpm start
     sudo service php-fpm status
     sudo service nginx status
     sudo yum install php-mysqlnd -y
     sudo systemctl enable nginx
     sudo systemctl enable php-fpm
     cd /usr/share/nginx/html/
     ls
     sudo nano pratham.html
     sudo nano upload.php
     sudo curl -sS https://getcomposer.org/installer | sudo php
     curl -sS https://getcomposer.org/installer | sudo php
     curl -sS https://getcomposer.org/installer | php
     sudo curl -sS https://getcomposer.org/installer | sudo php
     ls
     sudo nano upload.php
     sudo yum update
     sudo curl -sS https://getcomposer.org/installer | sudo php
     sudo yum install -y php-cli php-json php-zip curl unzip
     curl -sS https://getcomposer.org/installer | php
     sudo yum update
     sudo curl -sS https://getcomposer.org/installer | sudo php
     sudo service php-fpm status
     sudo systemctl enable php-fpm
     sudo systemctl status php-fpm
     sudo curl -sS https://getcomposer.org/installer | sudo php
     sudo mv composer.phar /usr/local/bin/composer
     sudo ln -s /usr/local/bin/composer /usr/bin/composer
     sudo composer require aws/aws-sdk-php
     cd
     sudo yum install mariadb105-server -y
     mysql -h s3-media.cnga6k4ocm0h.us-east-1.rds.amazonaws.com -u admin -p


create database facebook;
show databases;
use facebook;
create table users (id int primary key auto_increment, name varchar(100), surname varchar(100), gender varchar(100),email varchar(100), image_url varchar(100));
desc users;
select * from users;
exit

sudo service php-fpm reload
