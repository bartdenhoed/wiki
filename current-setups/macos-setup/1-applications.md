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
#### [1Password](https://1password.com/) (subscription)
> Password manager that keeps all passwords secure behind one password

*Saving all my credentials, tokens and other secret information, must have for every developer! (and other humans)*

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

#### [Cron](https://cron.com/) (freemium)
> Calendar for professionals and teams

*My calendar of choose, beautiful and with power tools!*

```bash
brew install --cask cron
```

#### [Google Chrome](https://www.google.com/chrome/) (free)
> Web browser

*This is my main browser for years.*

* Settings:
	* Menubar > Warn Before Quitting: On
* Extensions:
	* [1Password – Password Manager](https://chrome.google.com/webstore/detail/1password-x-%E2%80%93-password-ma/aeblfdkhhhdcdjpifhhbdiojplfjncoa)
	* [Application Launcher for Drive (by Google)](https://chrome.google.com/webstore/detail/application-launcher-for/lmjegmlicamnimmfhcmpkclmigmmcbeh)
	* [Google Docs Offline](https://chrome.google.com/webstore/detail/google-docs-offline/ghbmnnjooekpmoecnnnilnnbdlolhkhi)
	* [Google Meet Auto Disable Mic/Cam](https://chrome.google.com/webstore/detail/google-meet-auto-disable/dgggcpmnponfpgnifbdohajbdkbgjlhd)
	* [Google Search Keyboard Shortcuts](https://chrome.google.com/webstore/detail/google-search-keyboard-sh/iobmefdldoplhmonnnkchglfdeepnfhd)
	* [Grammarly for Chrome](https://chrome.google.com/webstore/detail/grammarly-for-chrome/kbfnbcaeplbcioakkpcpgfkobkghlhen)
	* [HTTPS Everywhere](https://chrome.google.com/webstore/detail/https-everywhere/gcbommkclmclpchllfjekcdonpmejbdp)
	* [I don’t care about cookies](https://chrome.google.com/webstore/detail/i-dont-care-about-cookies/fihnjjcciajhdojfnbdddfaoknhalnja)
	* [Matter](https://chrome.google.com/webstore/detail/matter/knjbgabkeojmfdhindppcmhhfiembkeb)
	* [Omni](https://chrome.google.com/webstore/detail/omni/mapjgeachilmcbbokkgcbgpbakaaeehi)
	* [Password Alert](https://chrome.google.com/webstore/detail/password-alert/noondiphcddnnabmjcihcjfbhfklnnep)
	* [Tracking Token Stripper](https://chrome.google.com/webstore/detail/tracking-token-stripper/kcpnkledgcbobhkgimpbmejgockkplob)
	* [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)
	* [Website IP](https://chrome.google.com/webstore/detail/website-ip/ghbmhlgniedlklkpimlibbaoomlpacmk)
* Tips:
	* [BrowserStack](https://chrome.google.com/webstore/detail/browserstack/nkihdmlheodkdfojglpcjjmioefjahjb)
	* [Dark Reader](https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh)
	* [JSON Formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa)
	* [Stylus](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
	* [Vue.js devtools](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
	* [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg)
	* [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm)
	* [Google Meet Enhancement Suite](https://chrome.google.com/webstore/detail/google-meet-enhancement-s/ljojmlmdapmnibgflmmminacbjebjpno)

```bash
brew install --cask google-chrome
```

#### [Google Chrome Canary](https://www.google.com/intl/en/chrome/canary/) (free)
> Web browser

*I like to do my development in a different browser on a separate chrome profile.*

* Settings:
	* Menubar > Warn Before Quitting: On

```bash
brew install --cask homebrew/cask-versions/google-chrome-canary
```

#### [Mimestream](https://mimestream.com/) (freemium)
> Native app email client for Gmail

*Still in beta but, much better than the standard Apple mail application.*

```bash
brew install --cask mimestream
```

#### [Pocket Casts](https://www.pocketcasts.com/) (free)
> Podcast platform

*My go-to cross platform podcast app for years.*

```bash
brew install --cask pocket-casts
```

#### [Bear](https://bear.app/) (subscription)
> Create, Tag, Export, Encrypt

*Bear is perfect for creating notes with Markdown support.*

```bash
mas install 1091189122
```

#### [Signal](https://signal.org/) (free)
> Instant messaging application focusing on security

*Secure messaging app, but I'm really don't use it that much as we should...*

```bash
brew install --cask signal
```

#### [Slack](http://slack.com/) (freemium)
> Team communication and collaboration software

*Necessary office tool to communicate with my colleagues.*

```bash
mas install 803453959
```

#### [Spotify](https://spotify.com) (freemium)
> Music streaming service

*For many years my cross platform music application.*

```bash
brew install --cask spotify
```

#### [Trello](https://trello.com/) (freemium)
> Organize anything, together

*With this tool, I managed a lot of projects to be on time.*

```bash
mas install 1278508951
```

#### [WhatsApp](https://www.whatsapp.com/) (free)
> Slimple. Reliable. Secure.

*My most used messaging application.*

```bash
mas install 1147396723
```

#### [Discord](https://discord.com/) (freemium)
> Voice and text chat software

*Chat app for gaming and (tech) communities.*

```bash
brew install --cask discord
```

#### [VLC](https://www.videolan.org/index.nl.html) (free)
> Multimedia player

*Best Open Source Video Player out there.*

```bash
brew install --cask vlc
```

#### [Brave Browser](https://brave.com/) (free)
> Web browser focusing on privacy

*I use this only for web development at this time.*

```bash
brew install --cask brave-browser
```

#### [Firefox](https://www.mozilla.org/firefox) (free)
> Web browser

*Also only used for web development.*

```bash
brew install --cask firefox
```

## Tools
#### [Google Drive](https://www.google.com/drive/download/) (freemium)
> Client for the Google Drive storage service

*Managing my files and media across all my devices.*

```bash
brew install --cask google-drive
```

#### [LuLu](https://objective-see.com/products/lulu.html) (free)
> Open-source firewall to block unknown outgoing connections

*Best free firewall for macOS.*

```bash
brew install --cask lulu
```

#### [Magnet](https://magnet.crowdcafe.com/) (paid)
> Organize Your Workspace

*Missing windows manager on macOS.*

```bash
mas install 441258766
```

#### [Netiquette](https://objective-see.com/products/netiquette.html) (free)
> Network monitor

```bash
brew install --cask netiquette
```

#### [Tunnelblick](https://tunnelblick.net/) (free)
> Free and open-source OpenVPN client

```bash
brew install --cask tunnelblick
```

#### [BalenaEtcher](https://www.balena.io/etcher/) (free)
> Tool to flash OS images to SD cards & USB drives

```bash
brew install --cask balenaetcher
```

#### [Bartender](https://www.macbartender.com/) (paid)
> Menu bar icon organizer

*Can't live without anymore.*

```bash
brew install --cask bartender
```

#### [Browserosaurus](https://browserosaurus.com/) (free)
> Open-source browser prompter

*Handy tool for choosing the right browser when opening a link when using multiple browsers.*

```bash
brew install --cask browserosaurus
```

#### [Raycast](https://www.raycast.com/) (free)
> Control your tools with a few keystrokes

*Best Spotlight replacement, even after using Alfred (alfredapp.com) for years.*

```bash
brew install --cask raycast
```

## Development
#### [iTerm2](https://iterm2.com/) (free)
> Terminal emulator as alternative to Apple's Terminal app

*Best terminal I ever used.*

* Settings:
	* General > Closing > Quit when all windows are closed: `On`
	* Appearance > General > Theme: `Minimal`
	* Appearance > Windows > Show window number in title bar: `Off`
	* Advanced > In the Minimal theme, how different should the background color of the selected tab be from the others: `0.02`
	* Advanced > in The Minimal theme, how prominent should split pane dividers be: `0`

```bash
brew install --cask iterm2
```

#### [Sublime Text](https://www.sublimetext.com/) (free)
> Text editor for code, markup and prose

*For simple text editing.*

TODO:
* Settings: [Preferences.sublime-settings]
* Packages: Theme - One Dark

```bash
brew install --cask sublime-text
```

#### [TablePlus](https://tableplus.com/) (paid)
> Native GUI tool for relational databases

*Favorite database client.*

```bash
brew install --cask tableplus
```

#### [Tower](https://www.git-tower.com/) (paid)
> Git client focusing on power and productivity

*Favorite Git client.*

```bash
brew install --cask tower
```

#### [VirtualBox](https://www.virtualbox.org/) (free)
> Virtualizer for x86 hardware

```bash
brew install --cask virtualbox
```

#### [Visual Studio Code](https://code.visualstudio.com/) (free)
> Open-source code editor

*Best code editor for web development.*

```bash
brew install --cask visual-studio-code
```

#### [Insomnia](https://insomnia.rest/) (freemium)
> HTTP and GraphQL Client

```bash
brew install --cask insomnia
```

#### [PHP Monitor](https://github.com/nicoverbruggen/phpmon) (free)
> A free, flexible, powerful tool that helps you monitor PHP Service.

*Shows my current PHP version in the menu bar.*

```bash
brew tap nicoverbruggen/homebrew-cask
brew install --cask phpmon
```

#### [DBngin](https://dbngin.com/) (free)
> Database version management tool

```bash
brew install --cask dbngin
```

#### [Tinkerwell](https://tinkerwell.app/) (paid)
> Tinker tool for PHP and Laravel developers

```bash
brew install --cask tinkerwell
```

#### [Docker](https://docker.com) (free)
> Pack, ship and run any application as a lightweight container

```bash
brew install --cask docker
```

#### [Ray](https://myray.app/) (paid)
> Debug with Ray to fix problems faster

```bash
brew install --cask ray
```

## Design
#### [Draw.io](https://app.diagrams.net/) (free)
> Draw.io is free online diagram software

```bash
brew install --cask drawio
```

#### [Figma](https://www.figma.com/) (freemium)
> Collaborative team software

```bash
brew install --cask figma
```

## Tips
#### [CleanMyMac X](https://cleanmymac.com/) (freemium)
> Tool to remove unnecessary files and folders from disk Chinese edition

```bash
brew install --cask cleanmymac
```

#### [ForkLift](https://binarynights.com/) (paid)
> Finder replacement and FTP, SFTP, WebDAV and Amazon s3 client

```bash
# https://binarynights.com/manual#fileviewer

$ defaults write com.apple.finder QuitMenuItem -bool true; killall Finder

brew install --cask forklift
```

#### [Intel Power Gadget](https://software.intel.com/content/www/us/en/develop/articles/intel-power-gadget.html) (free)
> Power usage monitoring tool enabled for Intel Core processors

```bash
brew install --cask intel-power-gadget
```

#### [iStat Menus](https://bjango.com/mac/istatmenus/) (paid)
> System monitoring app

```bash
brew install istat-menus
```

#### [Unshaky](https://github.com/aahung/Unshaky) (free)
> Software fix for double key presses on Apple's butterfly keyboard

```bash
brew install unshaky
```

#### [MacPass](https://macpassapp.org/) (free)
> Open-source, KeePass-client and password manager

```bash
brew install --cask macpass
```

#### [ProtonVPN](https://protonvpn.com) (subscription)
> VPN client focusing on security

```bash
brew install --cask protonvpn
```

#### [Folx](https://mac.eltima.com/download-manager.html) (free)
> Download manager with a torrent client

```bash
brew install --cask folx
```

#### [Next Meeting](https://apps.apple.com/us/app/next-meeting/id1017470484?mt=12) (free)
> Quickly see your next meeting

```bash
mas install 1017470484
```

#### [BlockBlock](https://objective-see.com/products/blockblock.html) (free)
> Monitors common persistence locations

```bash
brew install --cask blockblock
```

#### [Choosy](https://www.choosyosx.com/) (paid)
> Open links in any browser

```bash
brew install --cask choosy
```
