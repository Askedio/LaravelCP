# Laravel 5.1 Vendor Package Example
## An Example on how-to create a Vendor Package for Composer

This is the start of the LaravelCP project but it is a generic vendor package that you can install with composer.

This provides nearly all features of Laravel in your vendor package. You create your all of your site development as a vendor package instead of modifiying the base Laravel install.

# Before Installation
The install directions are how-to install this as my vendor package. Ideally you'll be cloning this and renaming it. I've not done this so I do not have the actual steps but it's like

* Clone the repo
* Rename Askedio/Laravelcp & askedio/laravelcp stuff to your namespace (search & replace all files)
* Rename files to match
* Rename shortucts for configs, lang, etc, they are "lcp::", so replace "lcp" in the alias loaders
* Add to a github repo
* Add to packagist.org
* Install with commands like below, but with your names and revisions

# Installation
## Add to composer.json
 
    "askedio/laravelcp": "laravel5-vendor-package",


## Register with config/app.php

    Askedio\Laravelcp\Providers\LaravelcpServiceProvider::class,

## Test

    php artisan serv

Browse to http://localhost:8000/dashboard

## Publish
        php artisan vendor:publish 
## Migrate
        php artisan migrate
## Seed
        php artisan db:seed 

# Using this package
You can use the 'base' version to rapidly develop vendor/composer based packages. Clone the git repo, rename it, rename the namespaces, and off you go! Now all of your Laravel code will be in your own vendor module :D

