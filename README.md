Heroku buildpack: FreeTDS
=======================

A Heroku Buildpack created to install [FreeTDS](http://www.freetds.org/) in your project.
Allows for usage of [TinyTDS](https://github.com/rails-sqlserver/tiny_tds) on Heroku.

Compatible with Heroku-12 stage.

Installation
----------------------
```bash
heroku buildpacks:add --index 1 https://github.com/maikomjames/heroku-buildpack-freetds.git
```

Configuration
----------------------
This buildpack will read the value of one configuration variable:

* **`FREETDS_SOURCE_URL`** - Path to a version of FreeTDS to install. Defaults to
    `https://www.freetds.org/files/stable/freetds-1.00.1.tar.gz`
