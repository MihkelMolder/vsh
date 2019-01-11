Tuleb paigaldada php ja mysql (pärast update ja upgrade käske)

käsud:

'apt install apt-transport-https'

'wget -O /etc/apt/trusted.gpg.d/php.gpg https://packages.sury.org/php/apt.gpg'

'apt install php5 php-pear php5-mysql'

'apt install mysql-server'



Nüüd tuleb konfigureerida ning kirjutada php keeles uus fail, millega saab

kujundada veebilehte (/var/www/html/pehape.php).

Siis saab minna veebiaadresile ning panna kaldkriibs ja pann .php faili nimi.

Kui 'phpmyadmin' on paigaldatud,s iis tuleb veebilehes minna serveri_ip/phpmyadmin

Panen pehape.php faili kausta /home/it/public_html

Loon samasse kausta faili info.php ning kirjutan sinna sisse rea:

< ?php phpinfo(); ? >
