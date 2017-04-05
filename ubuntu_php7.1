#!/bin/bash

# Update Package List
su root

apt-get update
apt-get upgrade -y

sudo apt-get install -y language-pack-en-base
locale-gen en_US.UTF-8

sudo apt-get install -y software-properties-common supervisor vim git git-flow git-core language-pack-zh*
sudo LC_ALL=en_US.UTF-8 add-apt-repository ppa:ondrej/php
sudo apt-get update

# Install php7.1
sudo apt-get install -y php7.1 php7.1-fpm php7.1-mysql php7.1-zip php7.1-curl php7.1-xml php7.1-mcrypt php7.1-json php7.1-gd php7.1-mbstring

sudo apt-get install -y php-redis php-ssh2
# Remove Apache2
sudo service apache2 stop
sudo apt-get remove apache2*
sudo apt-get autoremove
sudo apt-get autoclean

# Install Nginx
sudo apt-get -y install nginx
rm /etc/nginx/sites-enabled/default
rm /etc/nginx/sites-available/default
service nginx restart

# Set My Timezone
ln -sf /usr/share/zoneinfo/PRC /etc/localtime

# Install Composer
curl -sS https://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer

# Set Some PHP CLI Settings
sudo sed -i "s/error_reporting = .*/error_reporting = E_ALL/" /etc/php/7.1/cli/php.ini
sudo sed -i "s/display_errors = .*/display_errors = On/" /etc/php/7.1/cli/php.ini
sudo sed -i "s/post_max_size = .*/post_max_size = 10M/" /etc/php/7.1/cli/php.ini
sudo sed -i "s/upload_max_filesize = .*/upload_max_filesize = 10M/" /etc/php/7.1/cli/php.ini
sudo sed -i "s/;date.timezone.*/date.timezone = PRC/" /etc/php/7.1/cli/php.ini

# Setup Some PHP-FPM Options
sed -i "s/error_reporting = .*/error_reporting = E_ALL/" /etc/php/7.1/fpm/php.ini
sed -i "s/display_errors = .*/display_errors = On/" /etc/php/7.1/fpm/php.ini
sed -i "s/;cgi.fix_pathinfo=1/cgi.fix_pathinfo=0/" /etc/php/7.1/fpm/php.ini
sed -i "s/post_max_size = .*/post_max_size = 10M/" /etc/php/7.1/fpm/php.ini
sed -i "s/upload_max_filesize = .*/upload_max_filesize = 10M/" /etc/php/7.1/fpm/php.ini
sed -i "s/;date.timezone.*/date.timezone = PRC/" /etc/php/7.1/fpm/php.ini

service php7.1-fpm restart
