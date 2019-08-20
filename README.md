# Symfony4-LicenceDevWeb
Installation de Symfony 4
1) installer PHP 

2) Installer composer (voir https://getcomposer.org/)
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '93b54496392c062774670ac18b134c3b3a95e5a5e5c8f1a9f115f203b75bf9a129d5daa8ba6a13e2cc8a1da0806388a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
3) Création d'un nouveau projet symfony
```
composer create-project symfony/website-skeleton myproject
```
4) demarage du projet 
Rendez vous dans le dossier de votre projet et lancez votre serveur local 
```
cd mon-super-projet
php bin/console server:run
```
Votre projet est à présent disponible sur http://localhost:8000/
