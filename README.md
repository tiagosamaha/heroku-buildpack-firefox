Heroku buildpack: Firefox with geckodriver
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for [Firefox](http://www.mozilla.org/en-US/firefox/new/). Meant to be used in combination with something like xvfb, for headless operation.

Usage
-----

Example usage:

```shell
$ heroku create --stack cedar --buildpack http://github.com/evosystem-jp/heroku-buildpack-firefox

# or if your app is already created:
$ heroku buildpacks:add http://github.com/evosystem-jp/heroku-buildpack-firefox

$ git push heroku master
```