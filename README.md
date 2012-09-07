# Headless Jasmine Boilerplate

This is a starting place for those wanting to learn how to run headless Jasmine JavaScript tests locally and on Travis CI.

Once you're familiar with how it works, it should be easy to add to your own projects.

Project includes:

* how to setup Jasmine gem

* sample Jasmine layout, created via `jasmine init`

* tweak of Rakefile to use 'jasmine:ci' task by default (for Travis and other CI systems)

* Travis CI integration via .travis.yml -- see [Travis CI Getting Started](http://about.travis-ci.org/docs/user/getting-started/)

# Setup and seeing test runner in action

1. Clone this repository
    
2. Ruby should already be installed on your system. Or install via Homebrew (on OSX). Or use Ruby Version Manager (https://rvm.io) if you want to isolate these Ruby dependencies.

3. Make sure you're in the root of the repository (which contains the gem and rake files)
    
4. Install dependencies using bundler

        # run 'gem install bundler' if you don't already have bundler
        bundle install
    
5. Run tests

        bundle exec rake jasmine    # for a local web server version at http://localhost:8888
        bundle exec rake            # for default headless CI version. See "How to run headless" below.

## How to run headless (for Continuous Integration)

Headless CI requires additional dependencies.

If running on your own desktop, just install Firefox.

If running on a server:

1. a virtual framebuffer such as Xvfb

2. a headless DOM via such as `iceweasel on Ubuntu` (which is headless Firefox), PhantomJS, etc.

Travis CI has these dependencies installed (see .travis.yml file). If you're
running your own CI server, you'll need to install these.

# Are we running ok on Travis CI?

[![Build Status](https://secure.travis-ci.org/briangershon/headless-jasmine-boilerplate.png?branch=master)](http://travis-ci.org/briangershon/headless-jasmine-boilerplate)

# Helpful resources

* [Writing a CoffeeScript web application using TDD](http://watirmelon.com/2012/01/23/writing-a-coffeescript-web-application-using-tdd/)

* [Javascript Loves CI](http://www.zendesk.com/blog/javascript-loves-ci)

* [Travis CI Docs](http://about.travis-ci.org/docs/)
