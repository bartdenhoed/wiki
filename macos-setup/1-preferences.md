# Knowledge Base - macOS Setup - Preferences

### Table of contents
0. [Home](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/0-home.md)
1. [**Preferences**](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/1-preferences.md)
    - [System Preferences](#system-preferences)
    - [Dock](#dock)
    - [Touch Bar](#touch-bar)
    - [Menu Bar](#menu-bar)
    - [Finder](#finder)
    - [Desktop](#desktop)
    - [Emojis](#emojis)
2. [Configuration](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/2-configuration.md)
3. [Applications](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/3-applications.md)
4. [Local Development](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/4-local-development.md)
5. [Backup](https://github.com/bartdenhoed/wiki/blob/master/macos-setup/5-backup.md)

### System Preferences

##### Apple ID
- iCloud > iCloud Drive: System Preferences
- iCloud > Photos: On
- iCloud > Safari: On
- iCloud > Keychain: On
- iCloud > Find My Mac: On
- iCloud > Siri: On
- iCloud > Optimise Mac Storage: Off

##### General
- Appearance: Dark
- Show scroll bars: Automatically based on mouse or trackpad > When scrolling
- Prefer tabs: in full screen > always
- Allow Handoff between this Mac annd your iCloud devices: Off

##### Desktop & Screen Saver
- Desktop > Desktop Pictures: Big Sur Graphic
- Screen Saver > [Epoch Flip Clock](https://github.com/chrstphrknwtn/epoch-flip-clock-screensaver)
- Screen Saver > Screen Saver Options: Primary Display > All Displays
- Screen Saver > Start after: 20 Minutes > 10 Minutes

##### Dock & Menu Bar
- Dock & Menu Bar > Position on screen: Left
- Dock & Menu Bar > Automatically hide and show the Dock: On
- Dock & Menu Bar > Show recent applications in Dock: Off
- Wi-Fi > Show in Menu Bar: Off
- Bluetooth > Show in Menu Bar: On
- Sound > Show in Menu Bar: Always
- Battery > Show in Control Centre: On
- Clock > Use a 24-hour clock: On
- Clock > Display the time with seconds: On
- Spotlight > Show in Menu Bar: Off
- Siri > Show in Menu Bar: Off

##### Mission Control
- Automatically rearrange Spaces based on most recent use: Off
- Group windows by application: On
- Hot Corners > Left Top: Start Screen Saver
- Hot Corners > Right Top: Notification Center

##### Siri
- Enable Ask Siri: Off

##### Spotlight

##### Language & Region
- General > Preferred languages: English (US) & Dutch (Netherlands)
- General > Region: Netherlands

##### Notifications
##### Internet Accounts
##### Wallet & Apple Pay
##### Touch ID
##### Users & Groups
##### Accessibility
##### Screen Time
##### Extensions


##### Security & Privacy
- General > Require password: 5 minutes > 5 seconds
- General > Show a message when the screen is locked: [FULLNAME | PHONE | ADDRESS]
- FileVault > Turn On FileVault
- Firewall > Turn On Firewall

##### Software Update
- Automatically keep my Mac up to date: On

##### Network
##### Bluetooth

##### Sound
- Sound Effects > Select an alert sound: Boop
- Sound Effects > Alert volume: 75%
- Sound Effects > Show volume in menu bar: On

##### Printers & Scanners

##### Keyboard
- Keyboard > Key Repeat: Fast
- Keyboard > Delay Until Repeat: Short
- Keyboard > Turn keyboard backlight off after: 5 secs > 1 min
- Keyboard > Touch Bar shows: App Controls > Spaces
- Keyboard > Press Fn key to: Show F1, F2, etc. Keys > Expand Control Strip
- Keyboard > Customize Control Strip: Quick Actions, Screenshot, Space, Keyboard Brightness, Space, Media, Space, Brightness Slider, Mute, Volume Slider
- Keyboard > Modifier Keys: Caps Lock > Escape
--
- Text > Correct spelling automatically: Off
- Text > Capitalise words automatically: Off
- Text > Add full stop with double-space: Off
- Text > Use smart quotes and dashes: Off
- Text > for Double Quotes: "abc"
- Text > for Single Quotes: 'abc'
--
- Shortcuts > Keyboard > Move focus to next window: cmd + §
- Shortcuts > Spotlight > Show Spotlight search: Off
- Shortcuts > Spotlight > Show Finder search window: Off
- Shortcuts > Use keyboard navigation to move focus between controls: On
--
- Input Sources > U.S. International - PC & Dutch
- Input Sources > Show Input menu in menu bar: Off
--
- Dictation > Shortcut: Off

##### Trackpad
- Point & Click > Look up & data detectors: Off
- Point & Click > Tap to click: On
- Point & Click > Tracking speed: 4 > 8
- Point & Click > Force Click and haptic feedback: Off
--
- Scroll & Zoom > Scrol direction: Off
--
- More Gestures > Swipe between full-screen apps: Swipe left or right with three fingers > Swipe left or right with four fingers
- More Gestures > Mission Control: Swipe up with three fingers > Swipe up with four fingers
- More Gestures > App Exposé: Off > Swipe down with four fingers

##### Mouse

##### Displays
- Display > Resolution: Scaled - More Space
- Display > True Tone: Off
- Night Shift > Schedule: Custom (from 00:00 to 07:00)
- Night Shift > Color Temperature: More Warm

##### Battery
- Battery > Turn display off after: 2 min > 10 min
- Power Adapter > Turn display off after: 10 min > 30 min

##### Date & Time


##### Sharing
- Printer Sharing: On

##### Time Machine

##### Startup Disk




















### Dock

```
Remove all applications: `$ defaults write com.apple.dock persistent-apps -array`
I also add a little space between those apps and other open apps: `$ defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}'`

After that I change the speed off the dock animation to Super-fast.

Super-fast dock animation: `$ defaults write com.apple.dock autohide-time-modifier -float 0.12;`
No dock animation: `$ defaults write com.apple.dock autohide-time-modifier -int 0;`
Default dock animation: `$ defaults delete com.apple.dock autohide-time-modifier;`

To see this change run: `$ killall Dock;`
```

[image]

### Touch Bar
[image]

### Menu Bar
[image]

### Finder
##### Finder Preferences
- General > CDs, DVDs and iPods: Off
- General > New Finder windows show: [Home folder]
- Sidebar > Favorites: AirDrop, Applications, Desktop, Downloads, [home folder]
- Sidebar > iCloud: Off
- Sidebar > Locations: [Mac name], External disks, 'CDs, DVDs, and iOS Devices', Cloud Storage, Bonjour computers, Connected servers
- Advanced > Show all filename extensions: On
- Advanced > Show warning before changing an extension: Off
- Advanced > Show warning before removing from iCloud Drive: Off
- Advanced > Remove items from the Trash after 30 days: On
- Advanced > Keep folders on top > In windows when sorting by name: On
- Advanced > Keep folders on top > On Desktop: On
- Advanced > When performing a search: Search the Current Folder

##### View Options
- [Mac name] > Show item info: On

##### Menu bar
- View > Show Tab Bar
- View > Show Path Bar
- View > Show Status Bar

##### Sidebar
[image]

### Desktop
- Use Stacks: On
- Group By: Kind
- Sort By: Name


### Emojis
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
