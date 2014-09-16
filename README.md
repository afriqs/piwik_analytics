**!! WORK IN PROGRESS !!**

# PiwikAnalytics

**Note:** Original Gem from Fabian Becker. 
This is a fork of piwik_analytics version 1.0.2, because the outdated javascript.
It seams the orginal Github Repo is vanished and not more accessable.

The piwik_analytics gem provides an easy way to include Piwik into your application.
By default it will output the asynchronous piwik tracking code for every page
(given that it is configured correctly).

This another fork takes into accounts the french legislation and is compliant with the [CNIL requests](www.cnil.fr/vos-obligations/sites-web-cookies-et-autres-traceurs/outils-et-codes-sources/la-mesure-daudience/)

## Installation

Add `piwik_analytics` to Gemfile:

    gem 'piwik_analytics', '~> 1.0.5', :git => 'https://github.com/zzeroo/piwik_analytics.git'

Run `bundle install` and after this the generator:

    rails g piwik_analytics:install

This will install a piwik.yml configuration file into the `config` directory
of your application.


## Configuration

Open up `config/piwik.yml` and edit the settings. Each setting is described in
the config file itself.

## Usage

Inside your `application.html.erb` (or haml, slim) simply add

    <%= piwik_tracking_tag %>

Enjoy :)


# Licence
Released under MIT licence.
