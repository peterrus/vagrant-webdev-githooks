vagrant-webdev-githooks
===============

**Warning: these scripts are rather untested, use at your own risk, pull requests welcome**

Several githooks + installscript for various webdevelopment projects, they are meant to be downloaded instead of cloned.
Most commands are being run over 'vagrant ssh'

Installation
============

- Pick the contents of the directory for the application that you are using (drupal, wordpress, etc) and copy them to the root of your repository.
- modify the configuration file (hooks.conf)
- install the hooks using ./install_hooks while in the root of your repository **Warning: this will overwrite any hooks you have in this repository**

Hooks
=====

- Drupal (Requires Drush): exports your database before committing and imports it after a pull. Effectively putting your database under source-control (Only tested with MySQL).
- Wordpress (Requires wp-cli): exports your database before committing and imports it after a pull. Effectively putting your database under source-control (Only tested with MySQL).
