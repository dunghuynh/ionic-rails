# ionic-rails

ionic-rails wraps the [Ionic Framework](http://ionicframework.com/) library for use in Rails 4 and above. Assets will minify automatically during production.

    Note: This may not be a great idea at this point as Max Lynch points out the Ionic Framework doesn't have great cross-browser support. The goal of that project is to build packages that are wrapped for native device deployment. Because you aren't going to package up your backend rails implementation this isn't a good idea. If you want to use Rails with Ionic it's best to build your api and use a straight up implementation of Ionic.

## Usage

Add the following to your Gemfile:

    gem 'ionic-rails'

Add the following directives to your JavaScript manifest file:

    //= require angular/angular
    //= require angular/angular-animate
    //= require angular/angular-resource
    //= require angular/angular-sanitize
    //= require angular-ui/angular-ui-router
    //= require ionic
    //= require ionic-angular

Add the following directives to your Stylesheet manifest file:

    *= require ionic
    *= require themes/ionic-ios7

## Versioning

Every attempt is made to mirror the currently shipping Ionic version number wherever possible.

The major, minor, and patch version numbers will always represent the Ionic version.

## Breaking changes in v 0.9.25 

All ionic directives now has ion- prefix, e.g. <list> is now <ion-list> 
See http://forum.ionicframework.com/t/breaking-change-directives-will-now-be-prefixed-with-ion/1191

Ion Refresher - If you are using pull to refresh, you must change your code
See http://forum.ionicframework.com/t/breaking-change-ion-refresher-pull-to-refresh/1778
