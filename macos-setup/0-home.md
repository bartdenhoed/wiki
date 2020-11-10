# Knowledge Base - MacOS Setup - Home

### Introduction
Welcome to my MacOS web development setup on my MacBook Pro 16-inch 2019 (MacOS 11 Big Sur).

You will learn my favorite MacOS System Preferences, see the applications that I use every day and get the needed development software tools. All steps are detailed described below, but I use personally an automated script to install and configure all them all which can be found in automated-scripts.

---

### Table of contents
0. [**Home**](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/0-home.md)
1. [System Preferences](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/1-system-preferences.md)
2. [Homebrew](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/2-homebrew.md)
3. [Applications](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/3-applications.md)
4. [Configuration](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/4-configuration.md)
6. [Backup]

---

### Manual Setup
1. Setup clean install MacOS 11 Big Sur
2. Install Xcode Command Line Tools:
	- `xcode-select --install`
3. Clone GitHub Repository:
	- `git clone https://github.com/bartdenhoed/dotfiles.git .dotfiles`
	- username: `bartdenhoed`
	- password: `macos-setup-token`
4. Follow all steps described in this documentation

---

### Automated Setup
1. Setup clean install MacOS 11 Big Sur
2. Run Bootstrap script:
	- `cd .dotfiles`
	- `./bootstrap`

---

### TODO:

- Replace Atom packages with VS code plugins
- Composer: global Laravel


```
locate [filename]
git fetch --all && git reset --hard && git pull
```
