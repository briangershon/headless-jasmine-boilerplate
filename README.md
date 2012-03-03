# Headless Jasmine Boilerplate

This is a starting place for those wanting to learn how to run headless Jasmine JavaScript tests locally and on Travis CI.

Once you're familiar with how it works, it should be easy to add to your own projects.

Project demonstates:

* setting up Jasmine gem

* adding a sample Jasmine layout, created via `jasmine init`

* tweaking Rakefile to use 'jasmine:ci' task by default

* adding Travis CI integration via .travis.yml -- see [Travis CI Getting Started](http://about.travis-ci.org/docs/user/getting-started/)

# To see it in action

    # clone this repository
    
    # install dependencies using bundler (run 'gem install bundler' if you don't have bundler)
    bundle install
    
    # run tests
    rake

# Are we running ok on Travis CI?

[![Build Status](https://secure.travis-ci.org/briangershon/headless-jasmine-boilerplate.png?branch=master)](http://travis-ci.org/briangershon/headless-jasmine-boilerplate)

# Helpful resources

* [Writing a CoffeeScript web application using TDD](http://watirmelon.com/2012/01/23/writing-a-coffeescript-web-application-using-tdd/)

* [Javascript Loves CI](http://www.zendesk.com/blog/javascript-loves-ci)

* [Travis CI Docs](http://about.travis-ci.org/docs/)
