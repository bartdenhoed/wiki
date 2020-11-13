# Knowledge Base - macOS Setup - Home

![macos developer hero](https://github.com/bartdenhoed/knowledge-base/blob/master/images/macos_developer_hero.svg)

### Introduction
Welcome to my web development setup for macOS Big Sur. Currently I use this setup on a MacBook Pro 15" (2016) at home and a MacBook Pro 16" (2019) at work.

You will learn my favorite macOS preferences, see the applications that I use every day and get the development tools I use mostly for Laravel development. All steps are detailed described below. Also there is an automated script to install and configure most of these steps (under construction).

![macos big sur](https://github.com/bartdenhoed/knowledge-base/blob/master/images/macos_big_sur.png)

### Table of contents
0. [**Home**](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/0-home.md)
    - [Starting point](#starting-point)
    - [Automated Setup](#automated-setup)
    - [Preferences](#preferences)
    - [Configuration](#configuration)
    - [Applications](#applications)
    - [Local Development](#local-development)
    - [Backup](#backup)
1. [Preferences](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/1-preferences.md)
2. [Configuration](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/2-configuration.md)
3. [Applications](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/3-applications.md)
4. [Local Development](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/4-local-development.md)
5. [Backup](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/5-backup.md)

### Starting point
1. Fresh installation of macOS 11 Big Sur
2. You need the Command Line Tools for Xcode (includes `git`, `ssh`, `zip`, `vim` and others)
```bash
$ xcode-select --install
```
3. Clone GitHub Repository dotfiles:
	- `git clone https://github.com/bartdenhoed/dotfiles.git .dotfiles`
	- username: `bartdenhoed`
	- password: `macos-setup-token`
4. Homebrew installation
The Missing Package Manager for macOS: https://brew.sh/
```bash
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

### Automated Setup???????
Run Bootstrap script:
	- `cd .dotfiles`
	- `./bootstrap`

### Preferences

### Configuration

### Applications

### Local Development

### Backup

---

### TODO:

- Replace Atom packages with VS code plugins
- Composer: global Laravel


```
locate [filename]
git fetch --all && git reset --hard && git pull
```
