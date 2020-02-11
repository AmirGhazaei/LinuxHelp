
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
