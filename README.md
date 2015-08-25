Heroku buildpack: FreeTDS
=======================

A Heroku Buildpack created to install [FreeTDS](http://www.freetds.org/) in your project.
Allows for usage of [TinyTDS](https://github.com/rails-sqlserver/tiny_tds) on Heroku.

Installation
----------------------
```bash
heroku buildpacks:add --index 1 tdooner/heroku-buildpack-freetds
```

Configuration
----------------------
This buildpack will read the value of one configuration variable:

* **`FREETDS_SOURCE_URL`** - Path to a version of FreeTDS to install. Defaults to
    `ftp://ftp.freetds.org/pub/freetds/stable/freetds-1.00.tar.gz`


Testing
----------------------
```bash
heroku create --buildpack https://github.com/heroku/heroku-buildpack-testrunner
heroku buildpacks:add --index 1 heroku/ruby
```
