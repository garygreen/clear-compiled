Standalone `clear-compiled` command for Laravel 5
----

## Installation

1. Copy `clear-compiled` into your Laravel base directory (alongside `artisan`)
2. Replace instances of `php artisan clear-compiled` with simply `php clear-compiled` in your `composer.json`

## Why

The current Laravel artisan command relies on being able to bootstrap the framework to run the command. If your providers has changed, it may not be able to bootstrap Laravel and the command will fail with an exception `PHP Fatal error: Class ".../.../*ServiceProvider" not found.` This standalone `clear-compiled` command fixes that. :-)