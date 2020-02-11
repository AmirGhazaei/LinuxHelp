


1. Install LAMP-Server ([Link](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-ubuntu-18-04))
   1. `sudo apt install tasksel`
   1. `sudo tasksel install lamp-server`
   1. `sudo mysql_secure_installation`
   1. `sudo apt install php libapache2-mod-php php-mysql`
   1. `sudo apt install phpmyadmin php-mbstring php-gettext`
   1. `sudo gedit /etc/apache2/apache2.conf`
   1. Then add the following line to the end of the file.
      `Include /etc/phpmyadmin/apache.conf`
   1. `/etc/init.d/apache2 restart`
