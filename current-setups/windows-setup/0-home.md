# Wiki - Windows Setup - Home

<img src="/.images/macos_developer_hero.svg" width="500px" alt="macos developer hero">

## Introduction
Welcome to my game setup for Windows 11. Currently, I use a self-build pc (Intel Core i5-8600, Gigabyte GeForce GTX 1070 Ti in a Fractal Design Meshify C case) from 2018 at home.

You will learn my favorite Windows preferences, see the applications and tools that I use for mosly gaming. All steps are detailed described below. Also, there is an automated script to install and configure most of these steps.

*Tested on Windows 11 Pro (21H2)*

<img src="/.images/windows_11.png" width="200px" alt="windows 11">

## Table of contents
0. [**Home**](/current-setups/windows-setup/0-home.md)
    * [Required steps](#required-steps)
    * [Automated script](#automated-script)
    * [Manual setup](#manual-setup)
    * [Feedback](#feedback)
1. [Settings](/current-setups/windows-setup/1-settings.md)
2. [Applications](/current-setups/windows-setup/2-applications.md)
3. [Games](/current-setups/windows-setup/3-local-development.md)
4. [Backup](/current-setups/windows-setup/4-backup.md)

## Required steps
1. Fresh installation of [Windows 11](https://www.microsoft.com/windows/windows-11/)
2. [Chocolatey](https://chocolatey.org/) installation (The Package Manager for Windows)
```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

## Automated script
<!-- For further setup, you can use my automated bootstrap script or manually go through the next steps. Currently there are no scripts for the macOS System Preferences, so there for you need to follow the manual setup.
```bash
/bin/bash $HOME/.dotfiles/automated-scripts/bootstrap
``` -->

## Manual setup
Now you can proceed step by step and use what appeals to your wishes.

#### [1. Settings](/current-setups/windows-setup/1-settings.md)
In this step you will configure the Windows settings and also other things like the start menu.

<img src="/.images/windows_setup_settings.png" width="500px" alt="windows setup settings">

#### [2. Applications](/current-setups/windows-setup/2-applications.md)
If you used my automated script, all these applications are already installed and we are now going to adjust the settings.

<img src="/.images/windows_setup_startmenu.png" width="500px" alt="windows setup startmenu">

#### [3. Games](/current-setups/windows-setup/3-games.md)
When you're into gaming, these are my games.

<img src="/.images/windows_setup_games.png" width="500px" alt="windows setup games">

#### [4. Backup](/current-setups/windows-setup/4-backup.md)
A setup is only a good setup if you have good backups. I show you how I've set that up.

<img src="/.images/windows_setup_backup.png" width="500px" alt="windows setup backup">

## Feedback
If you have any questions, don't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |