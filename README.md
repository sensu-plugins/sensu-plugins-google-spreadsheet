## Sensu-Plugins-google-spreadsheet

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-google-spreadsheet.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-google-spreadsheet)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-google-spreadsheet.svg)](http://badge.fury.io/rb/sensu-plugins-google-spreadsheet)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-google-spreadsheet/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-google-spreadsheet)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-google-spreadsheet/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-google-spreadsheet)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-google-spreadsheet.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-google-spreadsheet)
[ ![Codeship Status for sensu-plugins/sensu-plugins-google-spreadsheet](https://codeship.com/projects/9904ed80-ea32-0132-7a33-32dfa18a9fce/status?branch=master)](https://codeship.com/projects/83076)

## Functionality

## Files
 * bin/handler-google-spreadsheet

## Usage

```
{
  "gsp": {
    "sheet": "Your SpreadShett ID",
    "username": "your_account@gmail.com",
    "apppassword": "Your Application Password"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-google-spreadsheet -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-google-spreadsheet`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-google-spreadsheet' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-google-spreadsheet' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
