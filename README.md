# Lemon

# Repository moved to https://github.com/Lemon-Framework/Lemon

Lemon is php micro framework built for simple applications.\
Latest version: 1.3.3\
Documentation: https://tenmajkl.github.io/docs.html

# Installation

Installation is provided via composer:\
`composer create-project lemon_framework/lemon:dev-master project-name`

Lemon doesn't use project generator, so you need to make files manually and run app using `php -S localhost:port`\
// Lemonade coming soon :)

# Minimal app

Here is code of simple app build only in index.php

```php    

<?php
require "vendor/autoload.php";


Route::get("/relative/(.+)/", function($var)
    {
        echo $var;
    });

Route::any("/", function()
    {
        echo "hi";
    });

Route::handler(404, function()
    {
        echo "404";
    });

Route::execute();

?>

```



