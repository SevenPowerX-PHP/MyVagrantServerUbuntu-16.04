# MyVagrantServerUbuntu-16.04
- [Как правильно писать программы на PHP7](https://www.youtube.com/watch?v=pDyVjREXSa4)
- [Введение в Vagrant](https://code.tutsplus.com/ru/tutorials/introduction-to-vagrant--cms-25917)


ssh -p 3333 user@46.63.8.118

sudo apt-get update

sudo apt-get install virtualbox-5.2

sudo apt-get update

sudo apt-cache show vagran

sudo apt-get install vagrant

mkdir MyVagrant

cd MyVagrant/

mkdir xenial64

cd xenial64/

vagrant init ubuntu/xenial64

ls 

должен появится  Vagrantfile файл

cat Vagrantfile

vagrant up

vagrant box update

- [Устаноаноноввка Vagrant на serveer ](https://howtoprogram.xyz/2016/07/23/install-vagrant-ubuntu-16-04/)

скачиваем пакет

wget https://download.virtualbox.org/virtualbox/5.2.18/virtualbox-5.2_5.2.18-124319~Ubuntu~xenial_amd64.deb

Устананоноавливаем скачианый пакет

sudo dpkg -i virtualbox-5.2_5.2.18-124319~Ubuntu~xenial_amd64.deb 

тоже проделываем с vagraant нужной верссии

[Устанавливаем PHP7.2](https://thishosting.rocks/install-php-on-ubuntu/)

Подключение по ssh

ssh-keygen

Generating public/private rsa key pair.

Enter file in which to save the key (/home/vagrant/.ssh/id_rsa): 

дОБАВЛЯЕМ Публичный ключ на GitHub

