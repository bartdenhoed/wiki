# Wiki - macOS Setup - Home

<img src="/.images/macos_developer_hero.svg" width="500px" alt="macos developer hero">

## Introduction
Welcome to my web development setup for macOS Monterey. Currently, I use this setup on a MacBook Pro 15" (2016) at home and a MacBook Pro 16" (2019) at work.

You will learn my favorite macOS preferences, see the applications that I use every day, and get the development tools I use mostly for Moodle & Laravel development. All steps are detailed described below. Also, there is an automated script to install and configure most of these steps.

*Tested on macOS version 12.0.1*

<img src="/.images/macos_monterey.png" width="200px" alt="macos monterey">

## Table of contents
0. [**Home**](/current-setups/macos-setup/0-home.md)
    * [Required steps](#required-steps)
    * [Automated script](#automated-script)
    * [Manual setup](#manual-setup)
    * [Feedback](#feedback)
1. [Configuration](/current-setups/macos-setup/1-configuration.md)
2. [Preferences](/current-setups/macos-setup/2-preferences.md)
3. [Applications](/current-setups/macos-setup/3-applications.md)
4. [Local Development](/current-setups/macos-setup/4-local-development.md)
5. [Backup](/current-setups/macos-setup/5-backup.md)

## Required steps
1. Fresh installation of [macOS 12 Monterey](https://www.apple.com/macos/monterey/)
2. You need the Command Line Tools for Xcode (includes `git`, `ssh`, `zip`, `vim` and other tools)
```bash
xcode-select --install
```
3. Cloning my (or your own) dotfiles [Dotfiles Template Repository](https://github.com/bartdenhoed/dotfiles-template):
```bash
git clone https://github.com/bartdenhoed/dotfiles.git $HOME/.dotfiles
```
4. [Homebrew](https://brew.sh/) installation (The Missing Package Manager for macOS)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## Automated script
For further setup, you can use my automated bootstrap script or manually go through the next steps. Currently there are no scripts for the macOS System Preferences, so there for you need to follow the manual setup.
```bash
/bin/bash $HOME/.dotfiles/automated-scripts/bootstrap
```

## Manual setup
Now you can proceed step by step and use what appeals to your wishes.

#### [1. Configuration](/current-setups/macos-setup/1-configuration.md)
Here starts the fun stuff. We're starting with the dotfiles and default directories and configure the terminal.

<img src="/.images/macos_setup_iterm_folders.png" width="500px" alt="macos setup iterm folders">

#### [2. Preferences](/current-setups/macos-setup/2-preferences.md)
In this step you will configure the macOS System Preferences and also other things like the touch bar, dock and launchpad.

<img src="/.images/macos_setup_preferences.png" width="500px" alt="macos setup preferences">

#### [3. Applications](/current-setups/macos-setup/3-applications.md)
If you used my automated script, all these applications are already installed and we are now going to adjust the settings.

<img src="/.images/macos_setup_launchpad.png" width="500px" alt="macos setup launchpad">

#### [4. Local Development](/current-setups/macos-setup/4-local-development.md)
When you're into web development, this is my setup mainly for [Laravel](https://laravel.com/).

<img src="/.images/macos_setup_vscode.png" width="500px" alt="macos setup vscode">

#### [5. Backup](/current-setups/macos-setup/4-local-development.md)
A setup is only a good setup if you have good backups. I show you how I've set that up.

<img src="/.images/macos_setup_backup.png" width="500px" alt="macos setup backup">

## Feedback
If you have any questions, don't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |