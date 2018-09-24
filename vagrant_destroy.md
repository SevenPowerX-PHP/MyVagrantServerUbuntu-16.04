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
           composer init 
           [https://packagist.org](https://packagist.org) кнопка submit
           
           git tag -a v1.0 -m"Version 1.0" версия библиотеки
           git push --tags
           на [https://packagist.org](https://packagist.org/packages/splx/dates) под надписью Find days number from birthday to today жмем update 
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
                 
           
           Host github.com
                  Hostname ssh.github.com
                  User vagrant
                  Port 443
                  IdentityFile ~/.ssh/id_rsa.pub
            
Edit Vagrantfile
                    
                    config.vm.synced_folder "project", "/home/vagrant/project"

        vagrant reload
        
   [Start PHPStorm project](https://habr.com/post/416359/)
   
   [Как удалить папку .idea и лишние файлы из Git ](https://gist.github.com/wpupru/0159fcb6f6bc903bdbe1ff3509a2847f)
        
        Как удалить папку .idea и лишние файлы из Git

        Удаляем ненужные папки и файлы при синхронизации в Git репозиторий

        Прежде всего добавим файл .gitignore в корень проекта:

        touch .gitignore

        Добавим в него построчно имена папок, которые необходимо исключить из синхронизации:

        echo ".idea","__pycache__" > .gitignore

        echo "__pycache__" > .gitignore

        Удалим все проиндексированные файлы:

        git rm -r -f --cached .

        Запустим индексацию заново:

        git add .

        Добавляем коммит и пушим:

        git commit -m "Remove files"
        git push -u origin master


        git commit -m "Python Starter"
