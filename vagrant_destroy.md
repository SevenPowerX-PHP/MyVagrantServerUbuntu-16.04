    vagrant destroy

    do-release-upgrade

      install the package maintainer's version                     │  
       │         keep the local version currently installed                   │  
       │         show the differences between the versions                    │  
       │         show a side-by-side difference between the versions          │  
       │         start a new shell to examine the situation 

      Выбираем install the package maintainer's version

    vagrant ssh-config (проверка конфигурации ssh)
    
   [PHP](https://thishosting.rocks/install-php-on-ubuntu/)
            
            sudo apt-get install php 
            php -v
            
      Install PHP 7.2 modules
         
            sudo apt-get install php-pear php-fpm php-dev php-zip php-curl php-xmlrpc php-gd php-mysql php-mbstring php-xml libapache2-mod-php
            
            To check all the PHP modules available in Ubuntu, run:
            
            sudo apt-cache search --names-only ^php
            
