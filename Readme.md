# Composer installer for Sledgehammer modules

Using this installer, all [Composer](http://getcomposer.org/) packages of `"type" : "sledgehammer-module"`
will be installed in `sledgehammer/` folder.

## Package requirements
Add the "sledgehammer/core" as dependancy to your package.

```
    "require": {
        "sledgehammer/core": "*"
    }
 ```

You can also use "sledgehammer/composer-installer" instead, but then "sledgehammer/core" won't be installed as dependancy 
(which the package probably relies on, being a "sledgehammer-module" and all)


## Installing Composer

```
curl -s https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin
```

##  Basic composer usage

```
cd  /your/project/
composer.phar install sledgehammer/core
```