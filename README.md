Heroku buildpack: Vert.x
========================

This is a fork of tomaslin's [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for [Vert.X](http://vertx.io/) apps.

This buildpack deploys with vertx.2.0.2-final. For detecting your app, it requires a vertx-marker file in your project's root directory.

If you do not provide a Procfile, your app is started with:

	vertx run server.groovy

Usage
-----

Example usage:

    $ ls
    vertx-marker

    $ heroku create APP_NAME -b https://github.com/metanet/heroku-buildpack-vertx-jdk7.git
	
	$ git push heroku master

    -----> Heroku receiving push
    -----> Fetching custom build pack... done
    -----> Vert.x app detected
    -----> Installing Vert.x..... done


