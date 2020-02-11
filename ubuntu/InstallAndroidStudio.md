
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
