# Cheat sheet


## Linux:
- Search in files: `grep -rnw '/path/to/somewhere/' -e "pattern"`

## MacOS
https://www.podfeet.com/blog/tutorials-5/encrypt-file-folder-osx/

- zip -e filename.encrypted ‘filename.png’
- zip -er foldername.encrypted ‘foldername’

- unzip -P ‘password’ filename.encrypted -d .
- unzip -P ‘password’ filename.encrypted -d encrypted

default password


#### MySQL
```
# Default Homebrew MySQL server config
[mysqld]
# Only allow connections from localhost
bind-address = 127.0.0.1
sql_mode=NO_ENGINE_SUBSTITUTION,ALLOW_INVALID_DATES
```


## Overige
URL: http://snazzylabs.com/article/5-killer-macos-tricks-hidden-in-terminal/

DOCK:
Super-fast animation: defaults write com.apple.dock autohide-time-modifier -float 0.12;
No animation: defaults write com.apple.dock autohide-time-modifier -int 0;
Revert to default: defaults delete com.apple.dock autohide-time-modifier;

defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'

killall Dock;



URL: http://snazzylabs.com/tutorial/five-advanced-tricks-for-mac-users/

Tip 1: Screenshot
defaults write com.apple.screencapture type jpg
 
Tip 2: Encrypt
encrypt (change path): openssl enc -aes-256-cbc -e -in {path-in} -out {path-out}
decrypt (change path): openssl enc -aes-256-cbc -d -in {path-in} -out {path-out}
 
Tip 3: Updates
defaults write com.apple.SoftwareUpdate ScheduleFrequency -int 1
 
Tip 5: Prevent sleep
caffeinate -i -t 3600




Avetica tar:
tar -czf(v) [filename].tar.gz [files]


Fix damaged applications:
- sudo spctl --master-disable
- sudo spctl --master-enable


Terminal commands:
 - defaults write com.apple.Terminal NSQuitAlwaysKeepsWindows -bool false

https://mallinson.ca/osx-web-development/


- defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'
- killall Dock

- defaults write com.apple.finder AppleShowAllFiles FALSE
- killall Finder





Change default screen capture type: defaults write com.apple.screencapture type jpg (TODO: In scrypt like mysql-secure-install)

Encrypt files: encrypt (change path): openssl enc -aes-256-cbc -e -in {path-in} -out {path-out}

Decrypt files: decrypt (change path): openssl enc -aes-256-cbc -d -in {path-in} -out {path-out}

Disable/enable Gatekeeper: sudo spctl --master-disable & sudo spctl --master-enable








install: brew install p7zip
compress: 7z a [filename].7z [folder]
uncompress: 7z x [filename].7z



usage: youtube-dl [url] (mp4)
usage: youtube-dl --extract-audio --audio-format mp3 [url] (mp3)

brew cleanup
xdebug
