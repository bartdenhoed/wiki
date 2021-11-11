# Wiki - macOS Setup - Preferences

<img src="/.images/macos_setup_preferences.png" width="500px" alt="macos setup preferences">

In this step you will configure the macOS System Preferences and also other things like the touch bar, dock and launchpad.

<img src="/.images/macos_monterey.png" width="200px" alt="macos monterey">

## Table of contents
0. [Home](/macos-setup/0-home.md)
1. [Configuration](/macos-setup/1-configuration.md)
2. [**Preferences**](/macos-setup/2-preferences.md)
    * [System Preferences](#system-preferences)
    * [Dock](#dock)
    * [Touch Bar](#touch-bar)
    * [Menu Bar](#menu-bar)
    * [Finder](#finder)
    * [Desktop](#desktop)
    * [Emojis](#emojis)
    * [Launchpad](#launchpad)
    * [Feedback](#feedback)
3. [Applications](/macos-setup/3-applications.md)
4. [Local Development](/macos-setup/4-local-development.md)
5. [Backup](/macos-setup/5-backup.md)

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
    - [ ] Siri
>
* Media & Purchases > Use Touch ID for Purchases: `On`

#### Familiy Sharing
-

#### General
* Appearance: `Dark`
* Sidebar icon size: `Large`
* Show scroll bars: `When scrolling`
* Prefer tabs: `always` when opening documents

#### Desktop & Screen Saver
* Desktop > Desktop Pictures: [Apple September Event 2021 - California Streaming](/.images/macos_background.png)
>
* Screen Saver > [Epoch Flip Clock](https://github.com/chrstphrknwtn/epoch-flip-clock-screensaver)
* Screen Saver > Screen Saver Options: `All Displays`
* Screen Saver > Start after: `10 Minutes`

#### Dock & Menu Bar
* Dock & Menu Bar > Position on screen: `Left`
* Dock & Menu Bar > Minimise windows intro application icon: `On`
* Dock & Menu Bar > Automatically hide and show the Dock: `On`
* Dock & Menu Bar > Show recent applications in Dock: `Off`
>
* Dock & Menu Bar > Clock > Display the time with seconds: `On`

#### Mission Control
* Automatically rearrange Spaces based on most recent use: `Off`
* Group windows by application: `On`
* Hot Corners > Left Top: `Start Screen Saver`
* Hot Corners > Right Top: `Notification Center`

#### Siri
* Enable Ask Siri: `Off`

#### Spotlight
-

#### Language & Region
* General > Preferred languages: `English (UK)` & `Dutch (Netherlands)`
* General > Region: `Netherlands`
* General > Advanced > Dates > Short: `01-06-2021`

#### Notifications & Focus
* Focus > Do Not Disturb > Turn On Automatically: `23:00 - 07:00`
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
* Add fingers

#### Keyboard
* Keyboard > Key Repeat: `Fast`
* Keyboard > Delay Until Repeat: `Short`
* Keyboard > Turn keyboard backlight off after: `1 min`
* Keyboard > Touch Bar shows: `Spaces`
* Keyboard > Press fn key to: `Show Emoji & Symbols`
* Keyboard > Press and hold fn key to: `Show App Controls`
* Keyboard > Customize Control Strip: Quick Actions, Screenshot, Space, Keyboard Brightness, Space, Brightness Slider, Mute, Volume Slider, Space, Media
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

#### Date & Time
-

#### Sharing
* Printer Sharing: `On`

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
dockutil --no-restart --add "/Applications/Google Chrome.app"
dockutil --no-restart --add "/Applications/Google Chrome Canary.app"
dockutil --no-restart --add "/Applications/Visual Studio Code.app"
dockutil --no-restart --add "/Applications/iTerm.app"
dockutil --no-restart --add "/Applications/Bear.app"
dockutil --no-restart --add "/Applications/Reminders.app"
dockutil --no-restart --add "/Applications/Spotify.app"
dockutil --no-restart --add "/Applications/Slack.app"
```

* Also adding a little space between those apps and other open apps
```bash
defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'
```

* After that I change the speed off the dock animation to fast or use no animation (super fast)
```bash
defaults write com.apple.dock autohide-time-modifier -float 0.1

defaults write com.apple.dock autohide-time-modifier -int 0
```

* To apply all these changes you must restart the Dock
```bash
killall Dock
```

* To undo, you can run this
```bash
defaults delete com.apple.dock
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
= Dollar character
```

## Launchpad

![launchpad](/.images/macos_setup_launchpad.png)

## Feedback
If you have any questions, don't hesitate to email my on contact[at]bartdenhoed.nl.

| [![github profile](/.images/me_pixar_small.png)](https://github.com/bartdenhoed) |
|---|
| [Bart den Hoed](https://github.com/bartdenhoed) |