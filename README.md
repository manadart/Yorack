Yorack
======

Simple setup for deploying a Yeoman application to Heroku with Rack.

### Getting Started

- Clone this repository.
- Set up [Yeoman](http://yeoman.io/index.html) and its dependencies.
- Scaffold a new site via ```yo webapp```.
- Make sure you have the necessary Ruby gems installed - Rack, Bundler etc.
- Copy the files from this repository into the root of your newly generated application.

### Deployment

- Run ```grunt build```.
- Follow [these instructions](https://github.com/yeoman/yeoman/wiki/Deployment) for deploying a Yeoman application via Git Subtree.
- Set the environment to production via ```heroku config:set RACK_ENV=production```.
- Push your Git Subtree (I use something like ```git subtree push --prefix dist heroku master```).

_Note: Working to figure out an issue with CoffeeScript files when running via Rack in development. It works fine in production._
