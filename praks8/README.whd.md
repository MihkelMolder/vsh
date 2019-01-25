#papo

Tegin uue kausta uue kausta sisse: 'mkdir /var/www/miguel.ee/public_html'
õigused:
'chown -R www-data /var/www/andres.ee'
'chgrp -R www-data /var/www/andres.ee'
Kausta sisse fail: 'touch index.html'
Kopeerida config fail apache kaustast: 'cp /etc/apache2/sites-available/000-default.conf /etc/apache2/sites-available/miguel.ee.conf'

#

Teen muudatusi selles failis:
'DocumentRoot /var/www/andres.ee
 ServerName andres.ee
 ServerAlias www.andres.ee'
 
'a2ensite /etc/apache2/sites-available/miguel.ee.conf'
'service apache2 restart'
