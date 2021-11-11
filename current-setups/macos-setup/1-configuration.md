# Wiki - macOS Setup - Configuration

## Table of contents
0. [Home](/macos-setup/0-home.md)
1. [**Configuration**](/macos-setup/1-configuration.md)
	* [Homebrew](#homebrew)
	* [Shell](#shell)
    * [Dotfiles](#dotfiles)
    * [Home directories](#home-directories)
    * [Fonts](#fonts)
    * [Feedback](#feedback)
2. [Preferences](/macos-setup/2-preferences.md)
3. [Applications](/macos-setup/3-applications.md)
4. [Local Development](/macos-setup/4-local-development.md)
5. [Backup](/macos-setup/5-backup.md)

## Homebrew
#### Formulas:
* [bat](https://github.com/sharkdp/bat) - Clone of cat with syntax highlighting and Git integration.
* [curl](https://curl.se/) - Get a file from an HTTP, HTTPS or FTP server.
* [diff-so-fancy](https://github.com/so-fancy/diff-so-fancy) - Good-lookin' diffs with diff-highlight and more.
<!-- * [dockutil](https://github.com/kcrawford/dockutil) - Command line utility for managing macOS dock items. -->
<!-- * [dnsmasq](https://thekelleys.org.uk/dnsmasq/doc.html) - Lightweight DNS forwarder and DHCP server. -->
* [ffmpeg](https://github.com/FFmpeg/FFmpeg) - Play, record, convert, and stream audio and video (required for converting videos with youtube-dl).
<!-- * [fontconfig](https://wiki.freedesktop.org/www/Software/fontconfig/) - XML-based font configuration API for X Windows -->
* [htop](https://htop.dev/) - Improved top (interactive process viewer).
* [mackup](https://github.com/lra/mackup) - Keep your application settings in sync.
* [mas](https://github.com/mas-cli/mas) - Command line interface for the Mac App Store.
* [speedtest-cli](https://github.com/sivel/speedtest-cli) - Command line interface for testing internet bandwidth.
* [tldr](https://github.com/tldr-pages/tldr) - Collaborative cheatsheet for console commands.
* [trash](https://github.com/ali-rantakari/trash) - CLI tool that moves files or folder to the trash.
* [wget](https://www.gnu.org/software/wget/) - Internet file retriever.
* [youtube-dl](https://github.com/l1ving/youtube-dl) - Download videos from youtube.com or other video platforms.


## Shell
#### Oh My Zsh
* Installation:
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

* Download custom theme and plugins:
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull
```

* Troubleshooting: fix permissions for Homebrew and Oh My Zsh:
```bash
sudo chown -R $(whoami) $(brew --prefix)/*
chmod 744 /usr/local/share/zsh
```

#### Vim (TODO)
* https://github.com/junegunn/vim-plug
* https://thevaluable.dev/vim-php-ide
* https://github.com/tpope/vim-sensible
```bash
# mkdir -p ~/.vim/pack/tpope/start
# cd ~/.vim/pack/tpope/start
# git clone https://tpope.io/vim/sensible.git
```

```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## Dotfiles
```bash
mv $HOME/.zshrc $HOME/.zshrc.backup

ln -s $HOME/.dotfiles/files/.editorconfig $HOME/.editorconfig
ln -s $HOME/.dotfiles/files/.gitattributes $HOME/.gitattributes
ln -s $HOME/.dotfiles/files/.gitconfig $HOME/.gitconfig
ln -s $HOME/.dotfiles/files/.gitignore $HOME/.gitignore
ln -s $HOME/.dotfiles/files/.mackup.cfg $HOME/.mackup.cfg
ln -s $HOME/.dotfiles/files/.my.cnf $HOME/.my.cnf
ln -s $HOME/.dotfiles/files/.p10k.zsh $HOME/.p10k.zsh
ln -s $HOME/.dotfiles/files/.vimrc $HOME/.vimrc
ln -s $HOME/.dotfiles/files/.zshrc $HOME/.zshrc

mkdir $HOME/.ssh
ln -s $HOME/.dotfiles/ssh/config $HOME/.ssh/config
```

## Home directories
```bash
mkdir $HOME/Desktop/Screenshots

mkdir $HOME/TEMP

mkdir $HOME/Projects
mkdir $HOME/Projects/laravel
mkdir $HOME/Projects/moodle
mkdir $HOME/Projects/kubernetes
mkdir $HOME/Projects/testing
mkdir $HOME/Projects/[company]
```

## Fonts
```bash
cp $HOME/.dotfiles/fonts/SourceCodePro+Powerline+Awesome+Regular.ttf /Library/Fonts/
```

## Screenshots
Save screenshots to a folder on the desktop:
```bash
defaults write com.apple.screencapture location -string "${HOME}/Desktop/Screenshots"
```

Disable shadow in screenshots
```bash
defaults write com.apple.screencapture disable-shadow -bool true
```

## Feedback
If you have any questions, don't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |