# Activity History

Sometimes its handy to know what your users are up to when they browse your app. The Activity Middleware and helper gives you everything you need to track your users and their every action. The middleware does most of it for you, but you're welcome to customize it to fit your needs. A great use case is documenting profile and billing changes. The activies logged in the database contain the request information, route, and the description passed to the method.

## Helper

```php-inline
activity($description) // will log the activity
```

## Middleware

The activity middleware simply runs the helper command stating a standard user action. This can easily be changed or removed if desired.

```php-inline
App\Middleware\Activity

activity('Standard User Action');
```
