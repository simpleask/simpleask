

```
sudo apt install php7.2-cli
```


```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'e0012edf3e80b6978849f5eff0d4b4e4c79ff1609dd1e613307e16318854d24ae64f26d17af3ef0bf7cfb710ca74755a') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```



```
sudo mv composer.phar /usr/local/bin/composer
```


```
composer require slim/slim:"4.*"
```

```
composer require slim/psr7
composer require nyholm/psr7 nyholm/psr7-server
composer require guzzlehttp/psr7 http-interop/http-factory-guzzle
composer require laminas/laminas-diactoros
```


```
cd public/
php -S localhost:8888
```

.htaccess
```
<IfModule mod_rewrite.c>
    RewriteEngine on
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteRule ^ index.php [QSA,L]
</IfModule>
```
