# Knowledge Base - MacOS Setup - System Preferences


##### Apple ID
- iCloud > iCloud Drive: System Preferences 
- iCloud > Safari: On
- iCloud > Keychain: On
- iCloud > Find My Mac: On
- iCloud > Optimise Mac Storage: Off

##### General
- Appearance: Dark
- Show scroll bars: Automatically based on mouse or trackpad > When scrolling
- Click in the scroll bar to: Jump to the spot that's clicked
- Allow Handoff between this Mac annd your iCloud devices: Off

##### Desktop & Screen Saver
- Desktop > Cataline: Dynamic
- Screen Saver > [Epoch Flip Clock](https://github.com/chrstphrknwtn/epoch-flip-clock-screensaver)
- Screen Saver > Show on: All Displays
- Screen Saver > Start after: 20 Minutes > 10 Minutes

##### Dock
- Position on screen: Left
- Prefer tabs when opening documents: In Full Screen Only > Always
- Automatically hide and show the Dock: On
- Show recent applications in Dock: Off

##### Mission Control
- Automatically rearrange Spaces based on most recent use: Off
- Group windows by application: On

##### Siri
- Enable Ask Siri: Off

##### Language & Region
- General > Preferred languages: English (UK) - Primary & Dutch (Netherlands)
- General > Region: Netherlands

##### Users & Groups


##### Accessibility
- Zoom > Use keyboard shortcuts to zoom: On
- Zoom > Use scroll gesture with modifier keys to zoom: On

##### Security & Privacy
- General > Require password: 5 minutes > immediately
- General > Show a message when the screen is locked: [FULLNAME | PHONE | ADRES]
--
- FileVault > Turn On FileVault
--
- Firewall > Turn On Firewall

##### Software Update
- Automatically keep my Mac up to date: On

##### Bluetooth
- Show Bluetooth in menu bar: On

##### Sound
- Sound Effects > Select an alert sound: Funk > Bottle
- Sound Effects > Alert volume: 75%
- Sound Effects > Show volume in menu bar: On

##### Keyboard
- Keyboard > Key Repeat: Fast
- Keyboard > Delay Until Repeat: Short
- Keyboard > Turn keyboard backlight off after: 5 secs > 1 min
- Keyboard > Press Fn key to: Show F1, F2, etc. Keys > Expand Control Strip
- Keyboard > Show keyboard and emoji viewers in menu bar: On
- Keyboard > Modifier Keys: Caps Lock > Escape
--
- Text > Correct spelling automatically: Off
- Text > Capitalise words automatically: Off
- Text > Add full stop with double-space: Off
- Text > Touch Bar typing suggestions: Off
- Text > Use smart quotes and dashes: Off
- Text > for Double Quotes: ""
- Text > for Single Quotes: ''
--
- Shortcuts > Keyboard > Move focus to next window: cmd + §
- Shortcuts > Spotlight > Show Spotlight search: Off
- Shortcuts > Spotlight > Show Finder search window: Off
- Shortcuts > Use keyboard navigation to mvoe focus between controls: On
--
- Input Sources > Dutch
- Input Sources > Show Input menu in menu bar: On
--
- Dictation > Shortcut: Off

##### Trackpad
- Point & Click > Look up & data detectors: Off
- Point & Click > Tap to click: On
- Point & Click > Click: Medium > Light
- Point & Click > Tracking speed: 4 > 7
- Point & Click > Force Click and haptic feedback: Off
--
- Scroll & Zoom > Scrol direction: Off
- Scroll & Zoom > Smart zoom: Off
--
- More Gestures > Swipe between full-screen apps: Swipe left or right with three fingers > Swipe left or right with four fingers
- More Gestures > Mission Control: Swipe up with three fingers > Swipe up with four fingers
- More Gestures > App Exposé: Off > Swipe down with four fingers

##### Displays
- Display > Resolution: More Space
- Display > True Tone: Off
- Display > Show mirroring options in the menu bar when available: Off

##### Energy Saver
- Batter > Turn display off after: 2 min > 10 min
--
- Power Adapter > Turn display off after: 10 min > 30 min

##### Date & Time
- Clock > Show date: On

##### Sharing
- Computer Name: "[Name]'s MacBook Pro" > "MacBook Pro van [Name]"

##### Time Machine
- Show Time Machine in mennu bar: On


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

### Touch Bar

### Menu Bar

### Finder
```
Preferences
General > Hard disks (On)
General > CD's, DVDs, and iPods (Off)
General > Connected servers (On)
General > New Finder windows shows: (Home folder)
Finder settings 1

Sidebar > Favorites > Applications (On)
Sidebar > Favorites > Desktop (On)
Sidebar > Favorites > Downloads (On)
Sidebar > Favorites > bartdenhoed (On)
Sidebar > Devices > Macbook Pro van Bart (On)
Sidebar > Devices > Hard disks (On)
Sidebar > Devices > External disks (On)
Sidebar > Devices > Connected servers (On)
Finder settings 2

Advanced > Show all filename extensions (On)
Advanced > Show warning before changing an extension (Off)
Advanced > Remove items from the Trash after 30 days (On)
Advanced > Keep folders on top: In windows when sorting by name & On Desktop (On)
Advanced > When performing a search: Search This Mac > Search the Current Folder
Finder settings 3

Menu bar
View > Show Tab Bar
View > Show Path Bar
View > Show Status Bar
Left bar
Finder left bar
```

### Desktop
```
Show View Options
Show item info (On)
Sort By (Snap to Grid)
```

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
```
