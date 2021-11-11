# Wiki - macOS Setup - Local Development

## Table of contents
0. [Home](/macos-setup/0-home.md)
1. [Configuration](/macos-setup/2-configuration.md)
2. [Preferences](/macos-setup/1-preferences.md)
3. [Applications](/macos-setup/3-applications.md)
4. [**Local Development**](/macos-setup/4-local-development.md)
    * [Required Software](#required-software)
    * [Laravel Valet](#laravel-valet)
    * [Laravel Sail](#laravel-sail)
5. [Backup](/macos-setup/5-backup.md)

## Required Software
#### Homebrew
```bash
# PHP
$ brew install php
$ brew install php@7.4
$ brew install php@7.2

# Composer
$ brew install composer
```

* [httpd](https://httpd.apache.org/) - Apache HTTP server
docker
aws-iam-authenticator
awscli
composer
nginx
mysql
php
php-cs-fixer
python
sqlite
terraform
git


#### Laravel Valet
```bash
$ composer global require laravel/valet

$ valet install
# $ valet tld local
$ valet use php@7.4

$ valet park $HOME/Projects/avetica
$ valet park $HOME/Projects/bartproductions
$ valet park $HOME/Projects/laravel
$ valet park $HOME/Projects/testing
```

```bash
$ ln -s $HOME/.dotfiles/.valet/Drivers/HugeValetDriver.php $HOME/.config/valet/Drivers/HugeValetDriver.php
$ ln -s $HOME/.dotfiles/.valet/Drivers/MoodleValetDriver.php $HOME/.config/valet/Drivers/MoodleValetDriver.php
```

#### Laravel Installer
```bash
$ composer global require laravel/installer

$ laravel new example-app
```

#### PHPUnit
```bash
$ brew install phpunit
```

## Laravel Valet
Using for development (SQLite)

## Laravel Sail
Using for acceptation test (MySQL)
