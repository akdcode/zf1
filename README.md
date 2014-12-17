Zend Framework 1 for Composer
=============================

This is a copy of the official Zend Framework 1 repository, with some modifications for improved [Composer](http://getcomposer.org/) integration.

## Why?

There are several reasons for using this package over of the official package:

* The following folders have been removed: `demos, documentation, externals, extras/documentation, extras/tests, src, tests`. This reduces the number of files from over 72000 to below 3500. It also reduces size from ~532MB to ~33MB.
* Improved autoloading. Explicit `require_once` calls in the source code has been commented out to rely on composer autoloading, this reduces the number of included files to a minimum.
* Composer integrates better with github than it does with subversion.

## How to use

Add `"akd/zf1": "1.*"` to the require section of your composer.json, include the composer autoloader and you're good to go.
