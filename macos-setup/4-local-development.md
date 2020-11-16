# Wiki - macOS Setup - Local Development

## Table of contents
0. [Home](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/0-home.md)
1. [Preferences](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/1-preferences.md)
2. [Configuration](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/2-configuration.md)
3. [Applications](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/3-applications.md)
4. [**Local Development**](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/4-local-development.md)
    - [Homebrew formulas](#homebrew-formulas)
5. [Backup](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/5-backup.md)


## Homebrew formulas


composer
DOCKER?

https://github.com/phpbrew/phpbrew


## Docker
# Docker Development

> https://medium.com/@yutafujii_59175/a-complete-one-by-one-guide-to-install-docker-on-your-mac-os-using-homebrew-e818eb4cfc3

#### Install Docker
- `brew install docker` (Client)
- `brew install docker-machine` (Daemon)
- `brew cask install virtualbox` (VM)

#### Create Virtual Machine
- New VM: `docker-machine create --driver virtualbox [vm-name]`
- List VM: `docker-machine ls`

#### Activate Docker
- `docker-machine env [vm-name]`
- `eval $(docker-machine env [vm-name]`

#### Testing
- `docker run hello-world`

#### Stop Virtual Machine
- `docker-machine stop [vm-name]`



## Laravel


## Laravel Valet
#### Install
- `composer global require laravel/valet`

#### Parks
```
# Parks
cd $HOME/Projects && valet park

# github
# laravel
# moodle
cd $HOME/Projects/development && valet park


```

#### Drivers
- `ln -s "$startdir/.valet/Drivers/HugeValetDriver.php" $HOME/.config/valet/Drivers/HugeValetDriver.php`

## MySQL

`mysql_secure_installation`
