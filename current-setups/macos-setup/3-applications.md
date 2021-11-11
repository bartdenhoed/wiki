# Wiki - macOS Setup - Applications

<img src="/.images/macos_setup_launchpad.png" width="500px" alt="macos setup launchpad">

If you used my automated script, all these applications are already installed and we are now going to adjust the settings.

## Table of contents
0. [Home](/current-setups/macos-setup/0-home.md)
1. [Configuration](/current-setups/macos-setup/1-configuration.md)
2. [Preferences](/current-setups/macos-setup/2-preferences.md)
3. [**Applications**](/current-setups/macos-setup/3-applications.md)
    * [General Usages](#general-usages)
    * [Tools](#tools)
    * [Development](#development)
    * [Design](#design)
    * [Tips](#tips)
4. [Local Development](/current-setups/macos-setup/4-local-development.md)
5. [Backup](/current-setups/macos-setup/5-backup.md)

## General Usages
#### [1Password](https://1password.com/)
Keeping all my password safe across all my devices.

* Settings:
	* General > Keyboard shortcuts > Show 1Password: Shift + CMD + \
	* General > Show item count in sidebar: On
	* Mini > Open 1Password to: Favourites
	* Mini > Categories: Show in submenu
	* Security > Require Master Password every: 1 week > 1 day
	* Security > Lock when main window is closed: On
	* Security > Lock after computer is idle for: 5 min > 60 min
	* Watchtower > Check for vulnerable passwords: On
	* Notifications > One-Time Passwords: Off
	* Notifications > Watchtower Alerts: On

```bash
brew install --cask 1password
```

#### [Google Chrome](https://www.google.com/chrome/)
Best browser for webdevelopment.

* Settings:
	* Menubar > Warn Before Quitting: On
* Extensions:
	* [1Password X – Password Manager](https://chrome.google.com/webstore/detail/1password-x-%E2%80%93-password-ma/aeblfdkhhhdcdjpifhhbdiojplfjncoa)
	* [Application Launcher for Drive (by Google)](https://chrome.google.com/webstore/detail/application-launcher-for/lmjegmlicamnimmfhcmpkclmigmmcbeh)
	* [Google Docs Offline](https://chrome.google.com/webstore/detail/google-docs-offline/ghbmnnjooekpmoecnnnilnnbdlolhkhi)
	* [Dark Reader](https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh)
	* [Google Search Keyboard Shortcuts](https://chrome.google.com/webstore/detail/google-search-keyboard-sh/iobmefdldoplhmonnnkchglfdeepnfhd)
	* [Grammarly for Chrome](https://chrome.google.com/webstore/detail/grammarly-for-chrome/kbfnbcaeplbcioakkpcpgfkobkghlhen)
	* [HTTPS Everywhere](https://chrome.google.com/webstore/detail/https-everywhere/gcbommkclmclpchllfjekcdonpmejbdp)
	* [I don’t care about cookies](https://chrome.google.com/webstore/detail/i-dont-care-about-cookies/fihnjjcciajhdojfnbdddfaoknhalnja)
	* [Notion Web Clipper](https://chrome.google.com/webstore/detail/notion-web-clipper/knheggckgoiihginacbkhaalnibhilkk)
	* [Password Alert](https://chrome.google.com/webstore/detail/password-alert/noondiphcddnnabmjcihcjfbhfklnnep)
	* [Tracking Token Stripper](https://chrome.google.com/webstore/detail/tracking-token-stripper/kcpnkledgcbobhkgimpbmejgockkplob)
	* [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)
	* [Website IP](https://chrome.google.com/webstore/detail/website-ip/ghbmhlgniedlklkpimlibbaoomlpacmk)
	* [Google Meet Enhancement Suite](https://chrome.google.com/webstore/detail/google-meet-enhancement-s/ljojmlmdapmnibgflmmminacbjebjpno)
	* [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa)
	* [Stylus](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
	* [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg)

```bash
brew install --cask google-chrome
```

#### [Google Chrome Canary](https://www.google.com/intl/en/chrome/canary/)

```bash
brew install --cask homebrew/cask-versions/google-chrome-canary
```

#### [Mimestream](https://mimestream.com/)
Favorite email client for Gmail.

```bash
brew install --cask mimestream
```

#### [Pocket Casts](https://www.pocketcasts.com/)
Cross-platform podcast client.

```bash
brew install --cask pocket-casts
```

#### [Bear](https://bear.app/)
Bear is perfect for creating notes with Markdown.

```bash
mas install 1091189122
```

#### [Signal](https://signal.org/)

```bash
brew install --cask signal
```

#### [Slack](http://slack.com/)

```bash
mas install 803453959
```

#### [Spotify](https://spotify.com)

```bash
brew install --cask spotify
```

#### [Trello](https://trello.com/)

```bash
mas install 1278508951
```

#### [WhatsApp](https://www.whatsapp.com/)

```bash
mas install 1147396723
```

#### [Discord](https://discord.com/)

```bash
brew install --cask discord
```

#### [VLC](https://www.videolan.org/index.nl.html)

```bash
brew install --cask vlc
```

#### [Brave Browser](https://brave.com/)

```bash
brew install --cask brave-browser
```

#### [Firefox](https://www.mozilla.org/firefox)
Only for web development testing.

```bash
brew install --cask firefox
```

## Tools
#### [Google Drive](https://www.google.com/drive/download/)
Synchronize all my important files.

```bash
brew install --cask google-drive
```

<!-- #### [BlockBlock](https://objective-see.com/products/blockblock.html) -->

#### [LuLu](https://objective-see.com/products/lulu.html)
LuLu is the free macOS firewall.

```bash
brew install --cask lulu
```

#### [Magnet](https://magnet.crowdcafe.com/)
Organize Your Workspace.

```bash
mas install 441258766
```

#### [Netiquette](https://objective-see.com/products/netiquette.html)

```bash
brew install --cask netiquette
```

#### [Tunnelblick](https://tunnelblick.net/)
Free software for OpenVPN on macOS.

```bash
brew install --cask tunnelblick
```

#### [BalenaEtcher](https://www.balena.io/etcher/)

```bash
brew install --cask lulu
```

#### [Bartender](https://www.macbartender.com/)
Organize your menu bar apps.

```bash
brew install --cask bartender
```

#### [Browserosaurus](https://browserosaurus.com/)
The browser prompter for macOS.

```bash
brew install --cask browserosaurus
```

#### [Raycast](https://www.raycast.com/)

```bash
brew install --cask raycast
```

#### [Next Meeting](https://apps.apple.com/us/app/next-meeting/id1017470484?mt=12)

```bash
mas install 1017470484
```

## Development
#### [iTerm2](https://iterm2.com/)
Best terminal ever.

* Settings:
	* General > Closing > Quit when all windows are closed: `On`
	* Appearance > General > Theme: `Minimal`
	* Appearance > Windows > Show window number in title bar: `Off`
	* Advanced > In the Minimal theme, how different should the background color of the selected tab be from the others: `0.02`
	* Advanced > in The Minimal theme, how prominent should split pane dividers be: `0`

```bash
brew install --cask iterm2
```

#### [Sublime Text](https://www.sublimetext.com/)
TODO:
* Settings: [Preferences.sublime-settings]
* Packages: Theme - One Dark

```bash
brew install --cask sublime-text
```

#### [TablePlus](https://tableplus.com/)

```bash
brew install --cask tableplus
```

#### [Tower](https://www.git-tower.com/)

```bash
brew install --cask tower
```

#### [VirtualBox](https://www.virtualbox.org/)

```bash
brew install --cask virtualbox
```

#### [Visual Studio Code](https://code.visualstudio.com/)

```bash
brew install --cask visual-studio-code
```

#### [Insomnia](https://insomnia.rest/)

```bash
brew install --cask insomnia
```

#### [PHP Monitor](https://github.com/nicoverbruggen/phpmon)


#### [DBngin](https://dbngin.com/)

```bash
brew install --cask dbngin
```

#### [Tinkerwell](https://tinkerwell.app/)

```bash
brew install --cask tinkerwell
```

#### [Docker](https://docker.com)

```bash
brew install --cask docker
```

#### [Ray](https://myray.app/)

```bash
brew install --cask ray
```

## Design
#### [Draw.io](https://app.diagrams.net/)

```bash
brew install drawio
```

## Tips

#### [CleanMyMac X](https://cleanmymac.com/)
Mac cleaner.

```bash
brew install cleanmymac
```

#### [ForkLift](https://binarynights.com/)
```bash
# https://binarynights.com/manual#fileviewer

$ defaults write com.apple.finder QuitMenuItem -bool true; killall Finder
```

#### [Intel Power Gadget](https://software.intel.com/content/www/us/en/develop/articles/intel-power-gadget.html)

#### [iStat Menus](https://bjango.com/mac/istatmenus/)

```bash
brew install istat-menus
```

#### [Unshaky](https://github.com/aahung/Unshaky)

```bash
brew install unshaky
```

#### [MacPass](https://macpassapp.org/)
A KeePass client for macOS.

#### [ProtonVPN](https://protonvpn.com)

#### [Folx](https://mac.eltima.com/download-manager.html)
