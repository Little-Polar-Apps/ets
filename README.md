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

Set DEFINED variables
===

You need to set the 'ets_source_read_handler' locations in order for ETS to know your templates directories, so that you are able to use {include:} and {insert:} correctly from your templates folder.

The function has already been included in ETS, but you will need to set the following defined variable:

```
define('ETS_TEMPLATESPATH', dirname(__FILE__) . '/templates');
```

Optionally
===

In addition to the source read handler two more functions are provided that set cache directory read and write. 

Set the file path as a defined variable 

```
define('ETS_THEMEFILEPATH', dirname(__FILE__));
```
