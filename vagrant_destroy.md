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
            
   Composer
           
           sudo apt-get install composer
           
  SSH подключение к GitHub
           
           ssh-keygen
           добавляем pub ключ на github
           
           если 22 порт закрыт используем 443
           [ностроем .ssh/config](https://www.cyberciti.biz/faq/create-ssh-config-file-on-linux-unix/)
           
           mkdir /Users/username/.ssh && chmod 700 /Users/username/.ssh
           touch /Users/username/.ssh/config
           nano /Users/username/.ssh/config
           
           Host github.com
                  Hostname ssh.github.com
                  Port 443
                  IdentityFile ~/.ssh/id_rsa.pub
            
