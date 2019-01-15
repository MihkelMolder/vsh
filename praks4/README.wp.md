Luban apache2-l kasutada ssl-i: 
'a2enmod ssl'
'a2ensite default-ssl'

Teen uue kausta ssl tsertifikaadi jaoks: 
'mkdir ssl'

Genereerin uue tsertifikaadi ja võtme et seda kaitsta: 
'openssl req -509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/apache2/ssl/apache.key -out /etc/apache2/ssl/apache.crt'

Soovikorral võiks panna turvalisuse mõttes õigused paika: 
'chmod 600 /etc/apache2/ssl/*'

Muudan faili sisu, et sätestada ssl-i kasutama: 
'nano /etc/apache2/sites-enabled/default-ssl.conf' 
Sisu: 

'SSLCertificateFile /etc/apache2/ssl/apache.crt'
'SSLCertificateKeyFile /etc/apache2/ssl/apache.key'

Restart apache.
