# Knowledge Base - macOS Setup - Home

![macos developer hero](https://github.com/bartdenhoed/knowledge-base/blob/master/.images/macos_developer_hero.svg)

## Introduction
Welcome to my web development setup for macOS Big Sur. Currently, I use this setup on a MacBook Pro 15" (2016) at home and a MacBook Pro 16" (2019) at work.

You will learn my favorite macOS preferences, see the applications that I use every day, and get the development tools I use mostly for Laravel development. All steps are detailed described below. Also, there is an automated script to install and configure most of these steps (under construction).

![macos big sur](https://github.com/bartdenhoed/knowledge-base/blob/master/.images/macos_big_sur.png)

## Table of contents
0. [**Home**](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/0-home.md)
    - [Required steps](#required-steps)
    - [Automated script](#automated-script)
    - [Next steps](#next-steps)
    - [Feedback](#feedback)
1. [Preferences](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/1-preferences.md)
2. [Configuration](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/2-configuration.md)
3. [Applications](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/3-applications.md)
4. [Local Development](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/4-local-development.md)
5. [Backup](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/5-backup.md)

## Required steps
1. Fresh installation of [macOS 11 Big Sur](https://www.apple.com/macos/big-sur/)
2. You need the Command Line Tools for Xcode (includes `git`, `ssh`, `zip`, `vim` and other tools)
```bash
$ xcode-select --install
```
3. Cloning my (or your own) dotfiles [GitHub Repository](https://github.com/bartdenhoed/dotfiles):
```bash
$ git clone https://github.com/bartdenhoed/dotfiles.git .dotfiles
```
4. [Homebrew](https://brew.sh/) installation (The Missing Package Manager for macOS)
```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## Automated script
For further setup, you can use my automated bootstrap script or manually go through the next steps.
```bash
$ cd .dotfiles
$ ./bootstrap
```

## Next steps
Now you can proceed step by step and use what appeals to your wishes.

#### [1. Preferences](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/1-preferences.md)
In this step you will configure the macOS System Preferences and also other things like the touch bar, dock and launchpad.

![screenshot preferences](https://github.com/bartdenhoed/knowledge-base/blob/master/.images/screenshot-preferences.png)

#### [2. Configuration](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/2-configuration.md)
Here starts the fun stuff. We're starting with the dotfiles and default directories and configure the terminal.

[image]

#### [3. Applications](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/3-applications.md)
If you used my automated script, all these applications are already installed and we are now going to adjust the settings.

[image]

#### [4. Local Development](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/4-local-development.md)
When you're into web development, this is my setup currently mainly for [Laravel](https://laravel.com/).

[image]

#### [5. Backup](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/4-local-development.md)
A setup is only a good setup if you have good backups. I show you how I've set that up.

[image]

## Feedback
If you have any questions, do't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](https://github.com/bartdenhoed/knowledge-base/blob/master/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |