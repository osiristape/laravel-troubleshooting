
## Laragon 
### upgrading php version
<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/php-1.png" height="80%" width="80%"/>
"Your Composer dependencies require a PHP version ">= 8.2.0". You are running ' . PHP_VERSION ."

- update PHP version from Laragon "PHP version 8.1.0" to "PHP version 8.3.0".
- download php-8.3.10 >> "https://windows.php.net/downloads/releases/php-8.3.10-nts-Win32-vs16-x64.zip"
- extract the zip file and paste here "Directory: C:\laragon\bin\php"
<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/php-2.png" height="30%" width="30%"/>

- check the version in terminal "php -v"
<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/php-3.png" height="30%" width="30%"/>
  
- right click and select PHP 8.3.10

or this one, i just put comment in php require version (example-app\vendor\composer\platform_check.php)

<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/php-4.png" height="50%" width="50%"/>

---
### Apache versioning
Apache: The procedure entry point nghttp2_option_set_no_rfc9113_leading_and_trailing_ws_validation could not be located in the dynamic link library.
- https://www.apachelounge.com/download/VS17/binaries/httpd-2.4.62-240718-win64-VS17.zip
- download httpd-2.4.62 zip file and extract
- move the entire files inside of "Apache24" folder to "httpd-2.4.62-240718-win64-VS17" (to make sure it is readable by laragon or terminal)
- copy the folder "httpd-2.4.62-240718-win64-VS17" and paste it "Directory: C:\laragon\bin\apache"
- select "httpd-2.4.62".
  <img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/httpd.png" height="30%" width="30%"/>

---
### MySQL
MySQL service can't start.

<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/mysql-1.gif" height="50%" width="50%"/>

- Download the ff:
  - MySQL Workbench: https://dev.mysql.com/downloads/file/?id=528765
  - MySQL Community Server 9.0.1
      - installer : https://dev.mysql.com/downloads/file/?id=531675
      - zip archive : https://dev.mysql.com/downloads/file/?id=531676
- install MySQL Workbench and mysqli 9.0.1 >> https://www.freecodecamp.org/news/how-to-install-mysql-workbench-on-windows/
- extract the zip file, copy mysql-9.0.1-winx64 and paste to "C:\laragon\bin\MySQL" and make sure it stores

<img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/mysql-2.png" height="20%" width="20%"/>

- open your terminal as administrator 
    "cd C:\laragon\bin\mysql\mysql-9.0.1-winx64\bin"
    "mysqld --initialize --datadir="C:\laragon\data\mysql-9" --basedir="C:\laragon\bin\mysql\mysql-9.0.1-winx64\bin" --console"
- open your file explorer.exe and paste this "C:\laragon\bin\mysql\mysql-9.0.1-winx64\bin\mysql_configurator.exe"

<img src="https://support.aparavi.com/wp-content/uploads/2023/08/sql81-scr8.png" height="40%" width="40%">
  
- mysql_configurator will ask you to fill up including the selected folder and password
- select "mysql-9.0.1-winx64"

  <img src ="https://github.com/osiristape/laravel-troubleshooting/blob/main/laragon-ver/mysql-3.png" height="30%" width="30%"/>

