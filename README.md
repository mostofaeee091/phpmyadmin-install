# phpmyadmin-install

apt update
sudo apt install phpmyadmin
sudo apt install php-mbstring php-zip php-gd php-json php-curl
cd /etc/apache2/
sudo nano apache2.conf
Include /etc/phpmyadmin/apache.conf
AllowOverride All
apt install mysql-server
sudo mysql
SELECT user.authentication_string,plugin,host FROM mysql.user;
CREATE DATABASE laravel_db;
CREATE USER 'laravel_user'@'localhost' IDENTIFIED BY 'admin007';
GRANT ALL ON laravel_db.* TO 'laravel_user'@'localhost';
FLUSH PRIVILEGES;
QUIT
