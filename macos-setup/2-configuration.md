# Knowledge Base - macOS Setup - Configuration

### Table of contents
0. [Home](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/0-home.md)
1. [Preferences](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/1-preferences.md)
2. [**Configuration**](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/2-configuration.md)
    - [Home symlinks](#home-symlinks)
    - [Directories](#directories)
3. [Applications](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/3-applications.md)
4. [Local Development](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/4-local-development.md)
5. [Backup](https://github.com/bartdenhoed/knowledge-base/blob/master/macos-setup/5-backup.md)

### Home symlinks
- Zshrc: `ln -s ~/dotfiles/.zshrc .zshrc`
- Git Config: `ln -s ~/dotfiles/.gitconfig .gitconfig`
- Git Ignore: `ln -s ~/dotfiles/.gitignore .gitignore`
- Editor Config: `ln -s ~/dotfiles/.editorconfig .editorconfig`


### Directories
- Temp:  `mkdir ~/Temp`
- STACK: `mkdir ~/STACK`
- Projects: `mkdir ~/Projects`
	- General:
		- `mkdir ~/Projects/general`
		- `echo "Projects/general" >> ~/Projects/general/index.html`
	- Development:
		- `mkdir ~/Projects/development`
		- `echo "Projects/development" >> ~/Projects/development/index.html`
	- [---]:
		- `mkdir ~/Projects/[---]`
		- `echo "Projects/[---]" >> ~/Projects/[---]/index.html`
```
git directories?
```


### Oh My Zsh
##### Themes
- `git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k`

##### Extensions
```
# colored-man-pages
# TODO ??????????
# extract
# TODO ??????????
# zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
# zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```


##### Fonts
```
cp "~/dotfiles/fonts/SourceCodePro+Powerline+Awesome+Regular.ttf" /Library/Fonts/
```

### Laravel


### Laravel Valet
##### Install
- `composer global require laravel/valet`

##### Parks
```
# Parks
cd $HOME/Projects && valet park

# github
# laravel
# moodle
cd $HOME/Projects/development && valet park


```

##### Drivers
- `ln -s "$startdir/.valet/Drivers/HugeValetDriver.php" $HOME/.config/valet/Drivers/HugeValetDriver.php`

### MySQL

`mysql_secure_installation`





```
locate [filename]
git fetch --all && git reset --hard && git pull
```


Maintenance:
- https://github.com/kristovatlas/osx-config-check
