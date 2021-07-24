# Umbrella Wireframe

Download a base for begin a new project based on Umbrella Wireframe

## MVC Model

Works with MVC PHP Concept

## Dependencies

To make the wireframe work, you have to install some dependencies, which are Composer, AltoRouter, Alto Dispatcher. 
And I always recommand Var Dumper to make Dumps more complete, and Dump and Die for an easier debug.

***Steps*** *All these commands in a shell on the root of your project*

1. Install Composer `composer require composer/composer`
2. Install Alto Router `composer require altorouter/altorouter`
3. Install Alto Dispatcher `composer require benoclock/alto-dispatcher`
4. If you want Var Dumper `composer require symfony/var-dumper`
5. Then go in the `composer.json` just made in your project, and after the dependencies, add this code for the namespaces:
```
    "autoload": {
        "psr-4": {"App\\": "app/"}
    }
```

Think to add the namespace at the begin of your pages ( Models, Controllers)

6. And to finish the config, make this command : `composer dump-autoload`
7. Don't forget to work with PHP Server on port 8080. You can use the server.sh
8. Make your config.ini, you have a model, just update it to connect you DB
9. Then you just have to start ^_^