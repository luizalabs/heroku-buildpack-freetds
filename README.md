Heroku buildpack: FreeTDS
=======================

A Heroku Buildpack created to install [FreeTDS](http://www.freetds.org/) in your project.
Allows for usage of [TinyTDS](https://github.com/rails-sqlserver/tiny_tds) on Heroku.

Compatible with Heroku-12 stage.

Installation
----------------------
```bash
heroku buildpacks:add --index 1 https://github.com/tdooner/heroku-buildpack-freetds.git
```

Configuration
----------------------
This buildpack will read the value of one configuration variable:

* **`FREETDS_SOURCE_URL`** - Path to a version of FreeTDS to install. Defaults to
    `ftp://ftp.freetds.org/pub/freetds/stable/freetds-1.00.tar.gz`
