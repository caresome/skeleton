# FilamentPHP Plugin Skeleton

[![Latest Version on Packagist](https://img.shields.io/packagist/v/caresome/skeleton.svg?style=flat-square)](https://packagist.org/packages/caresome/skeleton)
[![GitHub Tests Action Status](https://img.shields.io/github/actions/workflow/status/caresome/skeleton/run-tests.yml?branch=main&label=tests&style=flat-square)](https://github.com/caresome/skeleton/actions?query=workflow%3Arun-tests+branch%3Amain)
[![GitHub Code Style Action Status](https://img.shields.io/github/actions/workflow/status/caresome/skeleton/fix-php-code-style-issues.yml?branch=main&label=code%20style&style=flat-square)](https://github.com/caresome/skeleton/actions?query=workflow%3A"Fix+PHP+code+style+issues"+branch%3Amain)
[![Total Downloads](https://img.shields.io/packagist/dt/caresome/skeleton.svg?style=flat-square)](https://packagist.org/packages/caresome/skeleton)

This is a FilamentPHP plugin skeleton that you can use to build your own Filament v4 plugins. It comes pre-configured with everything you need to create panel plugins, standalone plugins, or both.

## Installation

```bash
composer require caresome/skeleton
```

```bash
php artisan skeleton:install
```

## Usage

Register the plugin in your panel provider:

```php
use Caresome\FilamentPluginSkeleton\SkeletonPlugin;

public function panel(Panel $panel): Panel
{
    return $panel
        ->plugins([
            SkeletonPlugin::make(),
        ]);
}
```

## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [Caresome](https://github.com/caresome)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.