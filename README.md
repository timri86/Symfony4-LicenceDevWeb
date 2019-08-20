# Symfony4-LicenceDevWeb
Installation de Symfony 4
1) Installer votre environnement de déveleppoment 
- EDI PHPStorm https://www.jetbrains.com/student/
- Wamp Server http://www.wampserver.com/

2) Installer PHP (Utilisateur Windows)

Si vous êtes sous Windows, votre PHP est sûrement bien installé mais Windows ne sait pas où le trouver, il faut juste le lui dire. Voici la démarche à suivre pour régler ce problème :

Allez dans les paramètres système avancés : Démarrer > Panneau de configuration > Système et sécurité > Système > Paramètres système avancés ;

- Cliquez sur le bouton  Variables d'environnement…  ;
- Regardez dans la section  Variables utilisateurs  ;
- Trouvez l'entrée  Path  et sélectionnez-la ;
- Cliquez sur  Modifier  ;
- Cliquez sur  Nouveau  puis entrez votre répertoire PHP à la fin. C'est le répertoire dans lequel se trouve le fichier  php.exe . Dans mon cas par exemple, je mets :  C:\wamp\bin\php\php7.1.0 ;
- Confirmez en cliquant sur OK. Vous devez ensuite redémarrer l'invite de commandes pour prendre en compte les changements.

3) Installer composer (voir https://getcomposer.org/)
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '93b54496392c062774670ac18b134c3b3a95e5a5e5c8f1a9f115f203b75bf9a129d5daa8ba6a13e2cc8a1da0806388a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
4) Céer nouveau projet symfony
```
composer create-project symfony/website-skeleton myproject
```
5) Demarrer votre projet 
Rendez vous dans le dossier de votre projet et lancez votre serveur local 
```
cd mon-super-projet
php bin/console server:run
```
Votre projet est à présent disponible sur http://localhost:8000/
