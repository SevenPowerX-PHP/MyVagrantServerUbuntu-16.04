[Быстрое рабочее окружение для web-разработчиков (Vagrant и PHPStorm)](https://habr.com/post/416359/)

(статья опубликована на [Linkedin](https://www.linkedin.com/pulse/configure-development-environment-learning-html-css-php-panov/))

  1. Cкачайте и установите Git для Windows [https://gitforwindows.org/](https://gitforwindows.org/).
  2. Устанавливаем на наш рабочий компьютер IDE PHPStorm, скачав его с [официального сайта](https://www.jetbrains.com/). 
  3. Установить на наш компьютер VirtualBox, скачав его с [официального сайта](https://www.virtualbox.org/). 
  4. Устанавливаем себе на компьютер Vagrant, скачав его с [официального сайта](http://www.vagrantup.com/downloads.html). 
     *   Если у вас появляется ошибка о несоответствии версии PowerShell, то обновите [Management Framework](https://www.microsoft.com/en-US/download/details.aspx?id=50395).
  5. Создаем себе рабочую папку, в которой и будем создавать наш сайт. Для примера это будет папка «webdev» на диске «С».
  6. mkdir webdev
  
     cd webdev
     
     git clone https://github.com/abyss-soft/webdev . (точка в конце обязательна копируем в текущий каталог)
  7. Перейдя в папку, вводим команду vagrant up. Консоль не закрываем. Когда мы поработаем и нам надо будет выключить виртуальный сервер, мы введем команду vagrant halt.
     *  Может потребоватся установить [VirtualBox Extension Pack](https://www.virtualbox.org/wiki/Downloads)  скачать - [All supported platforms](https://download.virtualbox.org/virtualbox/5.2.18/Oracle_VM_VirtualBox_Extension_Pack-5.2.18.vbox-extpack)
