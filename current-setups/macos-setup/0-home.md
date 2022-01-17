# Wiki - macOS Setup - Home

<img src="/.images/macos_developer_hero.svg" width="500px" alt="macos developer hero">

## Introduction
Welcome to my web development setup for macOS Monterey. Currently, I use this setup on a MacBook Pro 15" (2016) at home and a MacBook Pro 16" (2019) at work.

You will learn my favorite macOS preferences, see the applications that I use every day, and get the development tools I use mostly for Moodle & Laravel development. All steps are detailed described below. Also, there is an automated script to install and configure most of these steps.

*Tested on macOS version 12.1*

<img src="/.images/macos_monterey.png" width="200px" alt="macos monterey">

## Table of contents
0. [**Home**](/current-setups/macos-setup/0-home.md)
    * [Required steps](#required-steps)
    * [Automated scripts](#automated-scripts)
    * [Setup](#setup)
    * [Feedback & Credits](#feedback--credits)
1. [Configuration](/current-setups/macos-setup/1-configuration.md)
2. [Preferences](/current-setups/macos-setup/2-preferences.md)
3. [Applications](/current-setups/macos-setup/3-applications.md)
4. [Local Development](/current-setups/macos-setup/4-local-development.md)
5. [Backup](/current-setups/macos-setup/5-backup.md)

## Required steps
1. Fresh installation of [macOS 12 Monterey](https://www.apple.com/macos/monterey/)
```bash
sudo softwareupdate -i -a
```
2. You need the Command Line Tools for Xcode (includes `git`, `ssh`, `zip`, `vim` and other tools)
```bash
xcode-select --install
```
3. Cloning my (or your own) dotfiles [Dotfiles Template Repository](https://github.com/bartdenhoed/dotfiles-template):
```bash
git clone https://github.com/bartdenhoed/dotfiles.git $HOME/.dotfiles
```

## Automated scripts
You can use the Makefile for further setup, or continue right away with the manual steps below.
```bash
make -f ~/.dotfiles/Makefile
# /bin/bash $HOME/.dotfiles/script/macos-installation/bootstrap
# bash -c "`curl -fsSL https://raw.githubusercontent.com/bartdenhoed/dotfiles/master/remote-install.sh`"
```

<img src="/.images/macos_setup_automated_scripts.png" width="200px" alt="macos setup automated scripts">

## Setup
Now you can proceed step by step and use what appeals to your wishes.

#### [1. Applications](/current-setups/macos-setup/1-applications.md)
If you used my automated scripts, all these applications are already installed so we are now going to adjust some settings and fix the launchpad

[<img src="/.images/macos_setup_launchpad.png" width="500px" alt="macos setup launchpad">](/current-setups/macos-setup/1-applications.md)

#### [2. Preferences](/current-setups/macos-setup/2-preferences.md)
In this step you will configure the macOS System Preferences and also other things like the touch bar and dock. Most of these steps are already done with the automated scripts but unfortunately, some things need to be done manually.

[<img src="/.images/macos_setup_preferences.png" width="500px" alt="macos setup preferences">](/current-setups/macos-setup/2-preferences.md)

#### [3. Configuration](/current-setups/macos-setup/3-configuration.md)
Here starts the fun stuff. We're starting with the dotfiles, default directories and configure the terminal.

[<img src="/.images/macos_setup_iterm_folders.png" width="500px" alt="macos setup iterm folders">](/current-setups/macos-setup/3-configuration.md)

#### [4. Local Development](/current-setups/macos-setup/4-local-development.md)
When you're into web development, this is my setup mainly for [Laravel](https://laravel.com/).

[<img src="/.images/macos_setup_vscode.png" width="500px" alt="macos setup vscode">](/current-setups/macos-setup/4-local-development.md)

#### [5. Backup](/current-setups/macos-setup/5-backup.md)
A setup is only a good setup if you have good backups. I show you how I've set that up.

[<img src="/.images/macos_setup_backup.png" width="500px" alt="macos setup backup">](/current-setups/macos-setup/5-backup.md)

## Feedback & Credits
If you have any questions, don't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |
| 2021 - 2022 |

*Inspired by [webpro/dotfiles](https://github.com/webpro/dotfiles) & [mathiasbynens/dotfiles](https://github.com/mathiasbynens/dotfiles).*