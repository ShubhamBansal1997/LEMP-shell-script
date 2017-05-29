# LEMP Shell Script


It is a shell script to install LEMP stack on the ubuntu server [php,mysql,nginx].

  - Work on all cloud services (aws, digitalocean)
  - Easy to use
  - Setup in 2 mins
  - Work with most of php framworks and open scripts - Laravel, Codeigniter, Wordpress etc. 
  - Use php7.0 and most of the php packages(php7.0-mysql php7.0-fpm php7.0-mbstring php7.0-xml php7.0-curl php7.0-json mcrypt php7.0-mcrypt php7.0-zip )

# How to use !

  - In your ubuntu server 
    ```sh
    git clone git@github.com:ShubhamBansal1997/LEMP-shell-script.git
    cd LEMP-shell-script.git
    [sudo] chmod +x shell.sh
    ./shell.sh
    ```
  - LEMP Installation process started
  - First it ask for sudo status(you want to use superuser or not)[default_parameter]
    ```sh
    Use sudo[y]:y
    Enter your appname[hello-web]:testing
    Enter your domain name[mydomain.com]:testing.com
    Install mysql[y]:y
    Install Composer[y]: y
    Intialized git [y]: y
    Enter your server ip[127.0.0.1]:23.34.12.31
    ```
  - Please enter your ip correctly otherwise server will not work
  - Instalation process started it asked for various presmissions in between kept yes for them
  - If you install mysql it also asks
    ```sh
    Enter your database name[hello-web]:testing
    ```
  - If you intialized git then it asks
    ```sh
    If your adding ssh url please add your ssh keys!!!!!!!!!
    Git url[https://github.com/ShubhamBansal1997/LEMP-shell-script.git]:https://github.com/ShubhamBansal1997/LEMP-shell-script.git
    git branch would be addded to root directory 
    if you want to add make a pull request
    remove the default index.php
    rm -rf  index.php
    and then git pull your branch
    ```
    
Points to remember:
---
  - Please don't stop this after running otherwise you have to reset your server
  - Your nginx configuration can be edited here
    ```sh
    [sudo] nano /etc/nginx/conf.d/default.conf 
    ```
  - After changing your nginx configuration, restart ngnix
    ```sh
    [sudo] /etc/init.d/nginx restart
    ```
  - See error log of the server here
    ```sh
    cat /var/log/nginx/error.log
    ```
  - After making any change in php configuration.Run this
    ```sh
    [sudo] etc/init.d/php7.0-fpm restart
    ```

Note for Users
----

  - Post your requirements and error in issue
  - Would update as per needs and issues

License
----

MIT


**Free Software, Hell Yeah!**


