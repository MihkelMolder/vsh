uue masina ip on 172.23.13.38

1. 'su'

2. 'apt install apache2'

3. 'service apache2 start'

4. muudan index.html faili


nyyd tuleb teha public kaust:

1. 'mkdir /home/it/public_html'

2. 'ln -s /home/it/public_html /var/www'

3. 'a2enmod userdir'

4. 'service apache2 restart'

5. Profit!
