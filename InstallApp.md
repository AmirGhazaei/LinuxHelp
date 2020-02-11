1. Install jre and jdk in Ubuntu ([Link](https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-on-ubuntu-18-04))
   1. sudo apt install openjdk-8-jdk
   1. sudo gedit ~/.bashrc
   1. Add this line in the end of file
      1. `export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64`
      1. `export ANDROID_HOME=/usr/local/Android/Sdk`
      1. `export ANDROID_SDK_ROOT=/usr/local/Android/Sdk`
      1. `export PATH=${PATH}:${ANDROID_HOME}/tools`
      1. `export PATH=${PATH}:${ANDROID_HOME}/platform-tools`

1. Switch between java versions in ubuntu
    1. `sudo update-alternatives --config java`
    1. `Select java version`

1. Uninstall java
     1. `sudo apt-get purge openjdk-11*` (depending witch version)

1. Create Android Studio shortcut in desktop in ubuntu
   1. Open Gedit
   1. Pase the folowing code:
      ```
      [Desktop Entry]
      Version=1.0
      Type=Application
      Terminal=false
      Icon=/usr/local/android-studio/bin/studio.png
      Exec=sh /usr/local/android-studio/bin/studio.sh
      Name=Android Studio
      ```
   1. Now, save this file as AndroidStudio.desktop, to your desktop.
   1. `cd ~/Desktop && chmod a+x AndroidStudio.desktop`

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

1. Problem login to mysql in phpmyadmin: (ERROR 1698 (28000): Access denied for user 'root'@'localhost') ([Link](https://stackoverflow.com/questions/39281594/error-1698-28000-access-denied-for-user-rootlocalhost))
   1. `sudo mysql -u root -p`
   1. `ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'new-password';`
   1. `sudo service mysql stop`
   1. `sudo service mysql start`

1. Install PostgreSQL
   1. `sudo apt update`
   1. `sudo apt install postgresql postgresql-contrib`
   

   
