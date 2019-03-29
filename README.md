Heroku buildpack: Firefox with Geckodriver
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for [Firefox](http://www.mozilla.org/en-US/firefox/new/). Meant to be used in combination with something like xvfb, for headless operation.

Usage
-----

Example usage:

```shell
$ heroku create --stack cedar --buildpack http://github.com/evosystem-jp/firefox-buildpack

# or if your app is already created:
$ heroku config:add BUILDPACK_URL=http://github.com/evosystem-jp/firefox-buildpack

$ git push heroku master
```