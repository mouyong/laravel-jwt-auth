# LaravelJwtAuth extension

[![Latest Version on Plugin](https://img.shields.io/packagist/v/mouyong/laravel-jwt-auth.svg?style=flat-square)](https://packagist.org/packages/mouyong/laravel-jwt-auth)
[![Build Status](https://img.shields.io/travis/mouyong/laravel-jwt-auth/master.svg?style=flat-square)](https://travis-ci.org/mouyong/laravel-jwt-auth)
[![Quality Score](https://img.shields.io/scrutinizer/g/mouyong/laravel-jwt-auth.svg?style=flat-square)](https://scrutinizer-ci.com/g/mouyong/laravel-jwt-auth)
[![Total Downloads](https://img.shields.io/packagist/dt/mouyong/laravel-jwt-auth.svg?style=flat-square)](https://packagist.org/packages/mouyong/laravel-jwt-auth)

This is where your description should go. Try and limit it to a paragraph or two, and maybe throw in a mention of what PSRs you support to avoid any confusion with users and contributors.

## Installation

You can install the package via composer:

```bash
php artisan market:require mouyong/laravel-jwt-auth

composer require mouyong/laravel-jwt-auth
```

## Usage

单独使用登录功能是，请在 `auth()->login()` 时使用 Plugins\LaravelJwtAuth\Models\User，示例如下：

```php
use Plugins\LaravelJwtAuth\Models\User as JwtModelUser;

$user = \App\Models\User::first();

auth('api')->login(new JwtModelUser($user->toArray()));
```

``` php
// Usage description here
```

### Testing

``` bash
composer test
```

### How to create this package

`php artisan new LaravelJwtAuth`

Please see [plugin-manager](https://github.com/mouyong/plugin-manager) for more information.
