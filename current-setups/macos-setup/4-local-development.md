# Wiki - macOS Setup - Local Development

<img src="/.images/macos_setup_vscode.png" width="500px" alt="macos setup vscode">

When you're into web development, this is my setup mainly for [Laravel](https://laravel.com/).

## Table of contents
0. [Home](/current-setups/macos-setup/0-home.md)
1. [Configuration](/current-setups/macos-setup/1-configuration.md)
2. [Preferences](/current-setups/macos-setup/2-preferences.md)
3. [Applications](/current-setups/macos-setup/3-applications.md)
4. [**Local Development**](/current-setups/macos-setup/4-local-development.md)
    * [Required Software](#required-software)
    * [Laravel Valet](#laravel-valet)
    * [Laravel Sail](#laravel-sail)
5. [Backup](/current-setups/macos-setup/5-backup.md)

## Required Software
#### Homebrew
* git
* php
* composer
* nginx
* dnsmasq
* npm

```bash
brew install git
brew install composer
brew install nginx

# PHP
brew install php
brew install php@8.0
brew install php@7.4

# httpd
# docker
# aws-iam-authenticator
# awscli
# mysql
# php-cs-fixer
# python
# sqlite
# terraform
# phpunit
```

#### Composer
```bash
composer global require laravel/valet
composer global require laravel/installer
```

#### Laravel Valet
```bash
valet install

# valet tld local
# valet use php@7.4

# Register directories
valet park $HOME/Projects/laravel
valet park $HOME/Projects/moodle
valet park $HOME/Projects/blackhole
valet park $HOME/Projects/[company]

# Add custom drivers
ln -s $HOME/.dotfiles/.valet/Drivers/HugeValetDriver.php $HOME/.config/valet/Drivers/HugeValetDriver.php
ln -s $HOME/.dotfiles/.valet/Drivers/MoodleValetDriver.php $HOME/.config/valet/Drivers/MoodleValetDriver.php
```

#### NPM
```bash
npm install -g cross-env
```


## Laravel Valet
Using for development (SQLite)

## Laravel Sail
Using for acceptation test (MySQL)

## DigitalOcean
Production