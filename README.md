# heymrbass.com

[![Build Status](https://travis-ci.org/bergren2/heymrbass.com.svg?branch=master)](https://travis-ci.org/bergren2/heymrbass.com)

It's a site. About me.

## Environment Prereqs

You should have the following minimally setup:

- [Git](https://help.github.com/articles/set-up-git) (duh)
- [rbenv](https://github.com/sstephenson/rbenv)
& [ruby-build](https://github.com/sstephenson/ruby-build)

## Initial Project Setup

    $ git clone git@github.com:bergren2/heymrbass.git
    $ cd heymrbass
    $ rbenv install
    $ gem install bundler
    $ bundle install

## Development

Fire up

    $ bundle exec middleman server

and then check out the site at [localhost:4567](http://localhost:4567).

Even though this is a simple project, I use [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
to keep track of my changes. As such, please make any changes on and pull
requests against `develop`.

## Deployment

Travis takes care of continuous deployment.

### Caveats

If your directory is dirty, `git stash` before deploying.

If Rake complains about there already being an `origin` remote, remove the `build`
directory in its entirety.

## Configuration

After launching the development server, navigate to
[localhost:4567/__middleman/config](http://localhost:4567/__middleman/config)
for documentation on configuring Middleman. You should not have to relaunch the
server after making changes to `config.rb`.

## License

See LICENSE for details.
