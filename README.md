# Php-switcher

## Install the script :
`curl -L https://raw.githubusercontent.com/Thaldos/Php-switcher/master/sphp.sh > /usr/local/bin/sphp`


## To swtich to 7.1 :
`sudo nano /etc/apache2/apache2.conf`

```
LoadModule php7_module /home/linuxbrew/.linuxbrew/Cellar/php@7.1/7.1.32_1/lib/httpd/modules/libphp7.so
<FilesMatch \.php$>
        SetHandler application/x-httpd-php
</FilesMatch>
```

## To swtich to 7.3, Add to the end :
`sudo nano /etc/apache2/apache2.conf`

```
LoadModule php7_module /home/linuxbrew/.linuxbrew/Cellar/php/7.3.10/lib/httpd/modules/libphp7.so
<FilesMatch \.php$>
        SetHandler application/x-httpd-php
</FilesMatch>
```

`sphp 7.3`