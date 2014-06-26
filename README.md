ETS
===

Easy Template System for PHP

Originally developed by Franck Marcia adopted by Ian Tearle as template language of choice for Expanse CMS. 
The main ets.php serves as the default master copy of ETS, with this repoistory acting as a location for plugins and usage examples for other projects. 

It is not expected for the ets.php file to change much. If you spot anything that needs improvements please, fork and pull request.

Installation
===

Install Composer in your project:
```
    curl -s http://getcomposer.org/installer | php
```
Create a `composer.json` file in your project root:
``` json
{
    "require": {
        "little-polar-apps/ets": "dev-master"
    }
}
```
Install via Composer
```
php composer.phar install
```
