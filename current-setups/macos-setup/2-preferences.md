# Wiki - macOS Setup - Preferences

<img src="/.images/macos_setup_preferences.png" width="500px" alt="macos setup preferences">

In this step you will configure the macOS System Preferences and also other things like the touch bar, dock and launchpad.

## Table of contents
0. [Home](/current-setups/macos-setup/0-home.md)
1. [Applications](/current-setups/macos-setup/1-applications.md)
2. [**Preferences**](/current-setups/macos-setup/2-preferences.md)
    * [System Preferences](#system-preferences)
    * [Dock](#dock)
    * [Touch Bar](#touch-bar)
    * [Menu Bar](#menu-bar)
    * [Finder](#finder)
    * [Desktop](#desktop)
    * [Emojis](#emojis)
    * [Launchpad](#launchpad)
3. [Configuration](/current-setups/macos-setup/3-configuration.md)
4. [Local Development](/current-setups/macos-setup/4-local-development.md)
5. [Backup](/current-setups/macos-setup/5-backup.md)

## System Preferences

#### Apple ID
* iCloud:
    - [x] Photos
    - [x] Keychain
    - [x] iCloud Drive: only Shortcuts & iCloud Drive
    - [ ] iCloud Mail
    - [ ] Contacts
    - [ ] Calendars
    - [x] Reminders
    - [x] Notes
    - [x] Safari
    - [x] Find My Mac
    - [ ] Stocks
    - [x] Home
    - [x] Siri
>
* Media & Purchases > Use Touch ID for Purchases: `On`

#### Familiy Sharing
-

#### General
* Appearance: `Dark`
* Sidebar icon size: `Large`
* Allow wallpaper tinting in windows: `Off`
* Show scroll bars: `When scrolling`
* Prefer tabs: `always` when opening documents

```bash
defaults write NSGlobalDomain AppleInterfaceStyle "Dark"
defaults write NSGlobalDomain NSTableViewDefaultSizeMode 3
defaults write NSGlobalDomain AppleReduceDesktopTinting 1
defaults write NSGlobalDomain AppleShowScrollBars "When scrolling"
defaults write NSGlobalDomain AppleWindowTabbingMode "always"
```

#### Desktop & Screen Saver
* Desktop > Desktop Pictures: [Apple September Event 2021 - California Streaming](/.images/macos_background.png)
>
* Screen Saver > [Epoch Flip Clock](https://github.com/chrstphrknwtn/epoch-flip-clock-screensaver)
* Screen Saver > Screen Saver Options: `All Displays`
* Screen Saver > Start after: `10 Minutes`

```bash
defaults -currentHost write com.apple.screensaver idleTime 600
```

#### Dock & Menu Bar
* Dock & Menu Bar > Position on screen: `Left`
* Dock & Menu Bar > Minimise windows using: `Scale effect`
* Dock & Menu Bar > Minimise windows intro application icon: `On`
* Dock & Menu Bar > Automatically hide and show the Dock: `On`
* Dock & Menu Bar > Show recent applications in Dock: `Off`
>
* Dock & Menu Bar > Clock > Display the time with seconds: `On`

```bash
defaults write com.apple.dock orientation "left"
defaults write com.apple.dock mineffect "scale"
defaults write com.apple.dock minimize-to-application 1
defaults write com.apple.dock autohide 1
defaults write com.apple.dock show-recents 0
defaults write com.apple.menuextra.clock ShowSeconds 1
```

#### Mission Control
* Automatically rearrange Spaces based on most recent use: `Off`
* Group windows by application: `On`
* Hot Corners > Left Top: `Start Screen Saver`
* Hot Corners > Right Top: `Notification Center`

```bash
defaults write com.apple.dock mru-spaces 0
defaults write com.apple.dock expose-group-apps 1
defaults write com.apple.dock wvous-br-corner 1
defaults write com.apple.dock wvous-tl-corner 5
defaults write com.apple.dock wvous-tr-corner 12
```

#### Siri
* Enable Ask Siri: `Off`

#### Spotlight
-

#### Language & Region
* General > Preferred languages: `English (UK)` & `Dutch (Netherlands)`
* General > Region: `Netherlands`
* General > Advanced > Dates > Short: `01-06-2021`

```bash
defaults write NSGlobalDomain AppleLanguages -array "en-GB" "nl-NL"
defaults write NSGlobalDomain AppleLocale "en_NL"

defaults write NSGlobalDomain AppleICUDateFormatStrings -dict-add 1 "dd-MM-y"
defaults write NSGlobalDomain AppleLiveTextEnabled 1

# defaults write NSGlobalDomain AppleMeasurementUnits -string "Centimeters"
# defaults write NSGlobalDomain AppleMetricUnits -bool true
```

#### Notifications & Focus
* Focus > Work > Turn On Automatically: `09:00 - 17:00`

#### Internet Acconts
-

#### Passwords
-

#### Wallet & Apple Pay
-

#### Users & Groups
-

#### Accessibility
-

#### Screen Time
-

#### Extensions
-

#### Security & Privacy
* General > Require password: `5 seconds`
* General > Show a message when the screen is locked: `[FULLNAME | PHONE | ADDRESS]`
>
* FileVault > Turn `On` FileVault
>
* Firewall > Turn `On` Firewall

#### Software Update
* Automatically keep my Mac up to date: `On`

#### Network
-

#### Bluetooh
-

#### Sound
* Sound Effects > Select an alert sound: `Boop`
* Sound Effects > Alert volume: `75%`

#### Touch ID
-

#### Keyboard
* Keyboard > Key Repeat: `Fast`
* Keyboard > Delay Until Repeat: `Short`
* Keyboard > Turn keyboard backlight off after: `1 min`
* Keyboard > Touch Bar shows: `App Controls`
* Keyboard > Press fn key to: `Show Emoji & Symbols`
* Keyboard > Press and hold fn key to: `Expand Control Strip`
* Keyboard > Customize Control Strip
    - Control Strip: `Quick Actions, Brightness Slider, Volume Slider, Play/Pauze`
    - Expanded Control Strip: `Quick Actions, Show Desktop, Space, Keyboard Brightness, Space, Brightness Slider, Volume Slider, Mute, Space, Media`
* Keyboard > Modifier Keys > Caps Lock (⇪) Key: `⎋ Escape`
>
* Text > Correct spelling automatically: `Off`
* Text > Capitalise words automatically: `Off`
* Text > Add full stop with double-space: `Off`
* Text > Use smart quotes and dashes: `Off`
* Text > for Double Quotes: `"abc"`
* Text > for Single Quotes: `'abc'`
>
* Shortcuts > Keyboard > Move focus to next window: `⌘ + §`
* Shortcuts > Spotlight > Show Spotlight search: `Off`
* Shortcuts > Spotlight > Show Finder search window: `Off`
* Shortcuts > Use keyboard navigation to move focus between controls: `On`
>
* Input Sources > `Dutch`
>
* Dictation > Shortcut: `Off`

```bash
defaults write NSGlobalDomain InitialKeyRepeat 15
defaults write NSGlobalDomain KeyRepeat 2
defaults write com.apple.touchbar.agent PresentationModeGlobal "appWithControlStrip"


```

#### Trackpad
* Point & Click > Look up & data detectors: `Off`
* Point & Click > Tap to click: `On`
* Point & Click > Tracking speed: `8`
* Point & Click > Force Click and haptic feedback: `Off`
>
* Scroll & Zoom > Scrol direction: `Off`
>
* More Gestures > Swipe between full-screen apps: `Swipe left or right with four fingers`
* More Gestures > Mission Control: `Swipe up with four fingers`
* More Gestures > App Exposé: `Swipe down with four fingers`

#### Mouse
-

#### Displays
* Resolution > Scaled: `More Space`
>
* Night Shift > Schedule: `Custom` (from `00:00` to `07:00`)`
* Night Shift > Color Temperature: `More Warm`

#### Printers & Scanners
-

#### Sidecar
-

#### Battery
* Battery > Turn display off after: `10 min`
* Battery > Low power mode: `On`
>
* Power Adapter > Turn display off after: `30 min`
* Power Adapter > Prevent your Mac from automatically sleeping when the display is off: `On`

#### Date & Time
-

#### Sharing
* Computer Name: `[name] MacBook Pro [year]`
* Printer Sharing: `On`

```bash
sudo scutil --set ComputerName "$COMPUTER_NAME"
sudo scutil --set HostName "$COMPUTER_NAME"
sudo scutil --set LocalHostName "$COMPUTER_NAME"
sudo defaults write /Library/Preferences/SystemConfiguration/com.apple.smb.server NetBIOSName -string "$COMPUTER_NAME"
```

#### Time Machine
-

#### Startup Disk
-

## Dock
![dock](/.images/macos_setup_dock.png)

* First remove all default applications (Manually remove the Downloads folder)
```bash
defaults write com.apple.dock persistent-apps -array
```

* Add most used applications
```bash
dockutil --no-restart --add "/Applications/Mimestream.app"
dockutil --no-restart --add "/Applications/Cron.app"
dockutil --no-restart --add "/Applications/Bear.app"
dockutil --no-restart --add "/Applications/Google Chrome.app"
```

* Also adding a little space between those apps and other open apps
```bash
# defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'
dockutil --add '' --type spacer --section apps
```

* After that I change the speed off the dock animation to fast or use no animation (super fast)
```bash
# Fast
defaults write com.apple.dock autohide-time-modifier -float 0.1

# Super Fast
defaults write com.apple.dock autohide-time-modifier -int 0
```

* To undo, you can run this
```bash
defaults delete com.apple.dock
killall Dock
```

## Touch Bar
![touchbar normal](/.images/macos_setup_touchbar_normal.png)
![touchbar full](/.images/macos_setup_touchbar_full.png)

## Menu Bar
![menubar](/.images/macos_setup_menubar.png)

## Finder
<img src="/.images/macos_setup_finder.png" width="500px" alt="macos setup finder">

#### Finer Preferences
* General > CDs, DVDs and iPods: `Off`
* General > New Finder windows show: `'Home folder'`
>
* Sidebar > Favorites:
    - [ ] Recents
    - [x] AirDrop
    - [x] Applications
    - [x] Desktop
    - [ ] Documents
    - [x] Downloads
    - [ ] Movies
    - [ ] Music
    - [ ] Pictures
    - [x] 'Home folder'
* Sidebar > iCloud:
    - [ ] iCloud Drive
    - [ ] Shared
* Sidebar > Locations:
    - [x] 'MacBook Pro'
    - [ ] Hard disks
    - [x] External disks
    - [x] CDs, DVDs and iOS Devices
    - [x] Cloud Storage
    - [x] Bonjour computers
    - [x] Connected servers
* Sidebar > Tags:
    - [ ] Recent Tags
>
* Advanced > Show all filename extensions: `On`
* Advanced > Show warning before changing an extension: `Off`
* Advanced > Show warning before removing from iCloud Drive: `Off`
* Advanced > Remove items from the Bin after 30 days: `On`
* Advanced > Keep folders on top > In windows when sorting by name: `On`
* Advanced > Keep folders on top > On Desktop: `On`
* Advanced > When performing a search: `Search the Current Folder`

#### View Options on Home folder (Use as Defaults)
* Always open in list view: `On`
* Browse in list view: `On`
>
* Group By: `Kind`
* Sort By: `Name`
>
* Show item info: `On`
* Show Library Folder: `On`

#### Menu bar
* View > Show Tab Bar
* View > Show Path Bar
* View > Show Status Bar

#### Sidebar
Favourites:
* 'Home folder'
* Applications
* Desktop
* Downloads
* AirDrop
>
Locations:
* 'MacBook Pro'
* Network

#### Hidden options
```bash
# Expand save panel by default
defaults write NSGlobalDomain NSNavPanelExpandedStateForSaveMode -bool true
defaults write NSGlobalDomain NSNavPanelExpandedStateForSaveMode2 -bool true

# Expand print panel by default
defaults write NSGlobalDomain PMPrintingExpandedStateForPrint -bool true ?
defaults write NSGlobalDomain PMPrintingExpandedStateForPrint2 -bool true ?

# Save to disk (not to iCloud) by default
defaults write NSGlobalDomain NSDocumentSaveNewDocumentsToCloud -bool false ?

# Automatically quit printer app once the print jobs complete
defaults write com.apple.print.PrintingPrefs "Quit When Finished" -bool true ?

# Disable the “Are you sure you want to open this application?” dialog
defaults write com.apple.LaunchServices LSQuarantine -bool false

# Disable Resume system-wide
defaults write com.apple.systempreferences NSQuitAlwaysKeepsWindows -bool false

# Disable the crash reporter
defaults write com.apple.CrashReporter DialogType -string "none"
```

## Desktop
* Use Stacks: On

## Emojis
```
Emojis
Add this to the favorites:

ˆ = Control key (ctrl)
⌘ = Command key (cmd)
⌥ = Option key
⎋ = ESC key
⇧ = Shift key
⇪ = Caps lock key
⏎ = Return key
⌫ = Delete key
€ = Euro character
$ = Dollar character
```

## Launchpad

![launchpad](/.images/macos_setup_launchpad.png)
