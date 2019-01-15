Peab olema olemas php ja mysql masinas.

Teen uue databaasi ja kasutaja: 

'mysql -u root -p;'

'CREATE DATABASE wordpressbase;'

'CREATE USER wpusr@localhost IDENTIFIED BY "qwerty";'

'GRANT ALL PRIVILEGES ON wordpressbase.* TO spusr@localhost;'

'FLUSH PRIVILEGES;'

'exit;'

#

apache2 ja mysql restart


läheb /tmp kausta

laeb alla faili: 
'wget -c http://wordpress.org/latest/zip'
'apt install unzip'
'unzip -q latest.zip -d /var/www/html

#

Redigeerib õigusi: 

'chown -R it.www.data'

'chmod -R 755 /var/www/html/wordpress'

'mkdir -p /var/www/html/wordpress/wp-content/uploads'

'chown -R it.www-data /var/www/html/wordpress/wp-cantent/uploads'

#

Teen muudatusi failis /var/www/html/wordplress/wp-config.php. 
Muudan seal databaasi nime, kasutaja nime ning parooli.
