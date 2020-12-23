# Wiki - macOS Setup - Configuration

## Table of contents
0. [Home](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/0-home.md)
1. [Preferences](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/1-preferences.md)
2. [**Configuration**](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/2-configuration.md)
	* [Homebrew](#homebrew)
	* [Oh My Zsh](#oh-my-zsh)
    * [Dotfiles](#dotfiles)
    * [Home directories](#home-directories)
    * [Fonts](#fonts)
3. [Applications](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/3-applications.md)
4. [Local Development](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/4-local-development.md)
5. [Backup](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/5-backup.md)

## Homebrew
#### Formulas:
* [wget](https://www.gnu.org/software/wget/) - Internet file retriever.
* [bat](https://github.com/sharkdp/bat) - A cat(1) clone with syntax highlighting and Git integration.
* [htop](https://htop.dev/) - Improved top (interactive process viewer).
* [tldr](https://github.com/tldr-pages/tldr) - Collaborative cheatsheet for console commands.
* [trash](https://github.com/ali-rantakari/trash) - CLI tool that moves files or folder to the trash.
* [mackup](https://github.com/lra/mackup) - Keep your application settings in sync.
* [dockutil](https://github.com/kcrawford/dockutil) - Command line utility for managing macOS dock items.
* [mas](https://github.com/mas-cli/mas) - Command line interface for the Mac App Store.
* [speedtest-cli](https://github.com/sivel/speedtest-cli) - Command line interface for testing internet bandwidth.
* [youtube-dl](https://github.com/l1ving/youtube-dl) - Download videos from youtube.com or other video platforms.
* [ffmpeg](https://github.com/FFmpeg/FFmpeg) - Play, record, convert, and stream audio and video (required for converting videos with youtube-dl)

## Oh My Zsh
#### Install
```bash
$ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

#### Plugins
Custom theme and plugins
```bash
$ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
$ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
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
$ curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## Dotfiles
```bash
$ rm $HOME/.zshrc

$ ln -s $HOME/.dotfiles/.editorconfig $HOME/.editorconfig
$ ln -s $HOME/.dotfiles/.gitattributes $HOME/.gitattributes
$ ln -s $HOME/.dotfiles/.gitconfig $HOME/.gitconfig
$ ln -s $HOME/.dotfiles/.gitignore $HOME/.gitignore
$ ln -s $HOME/.dotfiles/.mackup.cfg $HOME/.mackup.cfg
$ ln -s $HOME/.dotfiles/.my.cnf $HOME/.my.cnf
$ ln -s $HOME/.dotfiles/.p10k.zsh $HOME/.p10k.zsh
$ ln -s $HOME/.dotfiles/.vimrc $HOME/.vimrc
$ ln -s $HOME/.dotfiles/.zshrc $HOME/.zshrc

$ mkdir $HOME/.ssh
$ ln -s $HOME/.dotfiles/.ssh/config $HOME/.ssh/config
```

## Home directories
```bash
$ mkdir $HOME/Desktop/screenshots

$ mkdir $HOME/TEMP

$ mkdir $HOME/Projects
$ mkdir $HOME/Projects/avetica
$ mkdir $HOME/Projects/testing
$ mkdir $HOME/Projects/laravel
$ mkdir $HOME/Projects/bartproductions
```

## Fonts
```bash
$ cp $HOME/.dotfiles/fonts/SourceCodePro+Powerline+Awesome+Regular.ttf /Library/Fonts/
```

## Screenshots
Save screenshots to a folder on the desktop:
```bash
$ defaults write com.apple.screencapture location -string "${HOME}/Desktop/screenshots"
```

Save screenshots in PNG format (other options: BMP, GIF, JPG, PDF, TIFF)
```bash
$ defaults write com.apple.screencapture type -string "png"
```

Disable shadow in screenshots
```bash
$ defaults write com.apple.screencapture disable-shadow -bool true
```

## Troubleshooting (TODO)
Fix permissions for Homebrew and Oh My Zsh:
```bash
$ sudo chown -R $(whoami) $(brew --prefix)/*
$ chmod 744 /usr/local/share/zsh
```

Maintenance:
* git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull
* https://github.com/kristovatlas/osx-config-check

TODO: Vimrc
