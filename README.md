# phpmyadmin-install

apt update <br>
sudo apt install phpmyadmin<br>
sudo apt install php-mbstring php-zip php-gd php-json php-curl<br>
cd /etc/apache2/<br>
sudo nano apache2.conf<br>
Include /etc/phpmyadmin/apache.conf<br>
AllowOverride All<br>
apt install mysql-server<br>
sudo mysql<br>
SELECT user.authentication_string,plugin,host FROM mysql.user;<br>
CREATE DATABASE laravel_db;<br>
CREATE USER 'laravel_user'@'localhost' IDENTIFIED BY 'admin007';<br>
GRANT ALL ON laravel_db.* TO 'laravel_user'@'localhost';<br>
FLUSH PRIVILEGES;<br>
QUIT
