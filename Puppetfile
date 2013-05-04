# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, :github_tarball => options[:repo]
end

# Includes many of our custom types and providers, as well as global
# config. Required.

github "boxen", "1.2.0"

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github "homebrew", "1.1.2"
github "ruby",     "3.1.0"
github "java",     "1.0.6"
github "macvim",   "1.0.0"
github "mongodb",  "1.0.0"
github "mysql",    "1.1.0"
github "phantomjs","1.0.0"
github "redis",    "1.0.0"
github "solr",     "1.0.0"
github "textmate", "1.1.0"
