# laravel-options-cors
Example middleware for laravel CORS headers if request method OPTIONS.
Working in Laravel >= 5.4, maybe 5.3.

## Using
For use OptionsCorsResponse middleware, copy it for your application and enable it in `Kernel::$middleware` array (but not in Kernel::$routeMiddleware, see https://github.com/laravel/framework/issues/19938).
### For example
```php
// App\Http\Kernel
// ...
protected $middleware = [
    // ...
    \App\Http\Middleware\OptionsCorsResponse::class,
];
```
Сhange `$headers` in `OptionsCorsResponse` if necessary.
