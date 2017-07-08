# suncalc

<!-- This file was generated by https://github.com/ypid/suncalc/blob/master/scripts/template. Do not edit this file directly but
     instead have a look at: ./metainfo.json, ./templates/ports_README.md.j2 at https://github.com/ypid/suncalc. -->

[![Build Status](https://travis-ci.org/ypid/suncalc.svg?branch=master)](https://travis-ci.org/ypid/suncalc)
[![BSD licensed](https://img.shields.io/badge/license-BSD-blue.svg)](https://tldrlegal.com/license/bsd-2-clause-license-%28freebsd%29)
[![haxelib version](https://img.shields.io/badge/Haxe-v1.7.0-blue.svg)](https://lib.haxe.org/p/suncalc)
[![NPM version](https://img.shields.io/npm/v/suncalc.svg)](https://www.npmjs.org/package/suncalc)
[![Packagist version](https://img.shields.io/packagist/v/ypid/suncalc.svg)](https://packagist.org/packages/ypid/suncalc)

[![GitHub stars](https://img.shields.io/github/stars/ypid/suncalc-php.svg?style=social&label=Star&maxAge=2592000)](https://github.com/ypid/suncalc-php/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/ypid/suncalc-php.svg?style=social&label=Fork&maxAge=2592000)](https://github.com/ypid/suncalc-php/network)
[![GitHub watchers](https://img.shields.io/github/watchers/ypid/suncalc-php.svg?style=social&label=Watch&maxAge=2592000)](https://github.com/ypid/suncalc-php/watchers)
[![GitHub open issues](https://img.shields.io/github/issues-raw/ypid/suncalc-php.svg?&maxAge=2592000)](https://github.com/ypid/suncalc-php/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/ypid/suncalc-php.svg?maxAge=2592000)](https://github.com/ypid/suncalc-php/issues?q=is%3Aissue+is%3Aclosed)
[![GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/ypid/suncalc-php.svg?&maxAge=2592000)](https://github.com/ypid/suncalc-php/pulls)
[![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed-raw/ypid/suncalc-php.svg?&maxAge=2592000)](https://github.com/ypid/suncalc-php/pulls?q=is%3Apr+is%3Aclosed)

[![PHPPackages Rank](https://phppackages.org/p/ypid/suncalc/badge/rank.svg)](https://phppackages.org/p/ypid/suncalc)
[![PHPPackages Referenced By](https://phppackages.org/p/ypid/suncalc/badge/referenced-by.svg)](https://phppackages.org/p/ypid/suncalc)
[![Packagist monthly downloads](https://img.shields.io/packagist/dm/ypid/suncalc.svg)](https://packagist.org/packages/ypid/suncalc)
[![Packagist daily downloads](https://img.shields.io/packagist/dd/ypid/suncalc.svg)](https://packagist.org/packages/ypid/suncalc)
[![Packagist total downloads](https://img.shields.io/packagist/dt/ypid/suncalc.svg)](https://packagist.org/packages/ypid/suncalc)


The SunCalc module allows to calculate sun position,
sunlight phases (times for sunrise, sunset, dusk, etc.),
moon position and lunar phase for the given location and time.

SunCalc was ported to [Haxe](https://en.wikipedia.org/wiki/Haxe) by [Robin `ypid` Schneider](https://github.com/ypid) to allow using it in a [planed rewrite of the opening hours library](https://github.com/opening-hours/opening_hours.js/issues/136).

It is based on the [JavaScript implementation](https://github.com/mourner/suncalc)
created by [Vladimir Agafonkin](http://agafonkin.com/en) ([@mourner](https://github.com/mourner))
as a part of the [SunCalc.net project](http://suncalc.net).

Most calculations are based on the formulas given in the excellent Astronomy Answers articles
about [position of the sun](http://aa.quae.nl/en/reken/zonpositie.html)
and [the planets](http://aa.quae.nl/en/reken/hemelpositie.html).
You can read about different twilight phases calculated by SunCalc
in the [Twilight article on Wikipedia](https://en.wikipedia.org/wiki/Twilight).

Refer to the [API documentation](https://ypid.github.io/suncalc/suncalc/SunCalc.html) for details.

## Install

Install the library for your favorite language by executing one of the following commands:

```Shell
haxelib install suncalc         # Haxe
npm install suncalc             # JavaScript/Node.JS
composer require ypid/suncalc   # PHP
```


## Getting started

Check out the following example to get started.

```php
## Needed when executed in the root of this repository.
require_once __DIR__ . '/lib/php/Boot.class.php';

## Needed when installed via composer. FIXME
# require_once __DIR__ . '/vendor/ypid/suncalc/lib/php/Boot.class.php';

echo suncalc_SunCalc::getMoonIllumination(new Date(2000, 1, 1, 0, 0, 0));
```

## TODO

Maintainer/tester with PHP knowledge wanted :wink:

Composer does provide a [autoload feature](https://getcomposer.org/doc/04-schema.md#autoload) which is currently not used.
My experience with PHP is very limited which is the reason I wrote in Haxe and
generated this PHP target only because all unit tests for PHP passed. If you
know how to properly support the autoload feature for this library, I will be
happy to integrate it.


## Internals
This library was automatically build using [Haxe](http://haxe.org/) to target PHP.

Refer to https://github.com/ypid/suncalc when you want to contribute. Note that you should only report issues against [the PHP target repository](https://github.com/ypid/suncalc-php) when you think the issue only applies to the PHP port of this library. If you are unsure, report [against the source repository](https://github.com/ypid/suncalc) instead.

## Unit testing

Unit testing is done [against the source repository](https://github.com/ypid/suncalc) in Haxe,
as well as against each transcompile target (PHP in this
case). You can check them out in the [source repository](https://github.com/ypid/suncalc).

## Maintainer

* [Robin Schneider](http://ypid.de/), role: Maintainer, Rewrite in Haxe



## License

[BSD-2-Clause](https://tldrlegal.com/license/bsd-2-clause-license-%28freebsd%29)
