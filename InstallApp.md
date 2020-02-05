1. Install jre and jdk in Ubuntu
  1.1. sudo apt install openjdk-8-jdk
  1.1. sudo gedit ~/.bashrc
  1.1. Add this line in the end of file
    1.1.1. export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
    1.1.1. export ANDROID_HOME=/usr/local/Android/Sdk
    1.1.1. export ANDROID_SDK_ROOT=/usr/local/Android/Sdk
    1.1.1. export PATH=${PATH}:${ANDROID_HOME}/tools
    1.1.1. export PATH=${PATH}:${ANDROID_HOME}/platform-tools
useful link: https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-on-ubuntu-18-04 

2. Switch between java versions in ubuntu
  2.1. sudo update-alternatives --config java
  2.2. Select java version

3. Uninstall java
  3.1. sudo apt-get purge openjdk-11* (depending witch version)

4. Create Android Studio shortcut in desktop in ubuntu
  4.1. Open Gedit
  4.2. Pase the folowing code:
      ```
      [Desktop Entry]
      Version=1.0
      Type=Application
      Terminal=false
      Icon=/usr/local/android-studio/bin/studio.png
      Exec=sh /usr/local/android-studio/bin/studio.sh
      Name=Android Studio
      ```
  4.3. Now, save this file as AndroidStudio.desktop, to your desktop.
  4.4. cd ~/Desktop && chmod a+x AndroidStudio.desktop
