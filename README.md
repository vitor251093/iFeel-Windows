# macOsFeel (Windows)
\[WIP\] Scripts and Apps to mimic the macOS Mojave feel in Windows 10

**WARNING: None of the stuff mentioned below was done yet. Consider this as the plans for a new project**

## Modules
macOsFeel tries to mimic the macOS appearance and functionalities, but each part of it is an individual app or script, and they are not dependent of each other. Here, you will find the modules names, so you can check exactly what are you looking for. 

Be warned: this is being created for personal use, focusing in my macOS experience, and the feature that I would miss the most while migrating to a Windows computer. In case you miss anything, submit a pull request with the change.

### Dock
There are many applications that mimic the macOS dock in Windows, but most of them ignore its functionalities. The functionalities that I intent to implement are:
- Three groups in the Dock: Finder+apps, recent apps and folders+bin
- macOS right-click options for apps and folders (Open/Close, Options, ...)
- The ability to navigate throught the folders using the Dock in Fan, Grid or List style.
- An Applications folder in the Dock, allowing the user to launch an app on click, or launch its unninstaller in silent mode by dragging it to the bin (this is not the same thing as the Launchpad).
- Showing minimized windows in the corner, if it's configured to do so.
- Showing a small white dot below the opened applications.
- The capability to add new apps/folders with drag-and-drop.
- The capability to move apps/folders in the Dock with drag-and-drop.
- In the recent apps area, show a minimum of three apps.

### Menubar
The macOS menubar can't be perfectly recreated in Windows since the menubar of Windows application is inside their own windows, but that doesn't mean we can't have a menubar. The functionalities that I intent to implement in the left side are:
- Showing a Windows flag menu (for the same system-related options found in the macOS's Apple menu).
- Showing the app name menu, with the common options: About, Preferences..., Hide App, Hide Others, Show All, Quit App.
- Showing the Window menu, with the common options.
- When clicking in the app name menu -> Preferences... button, the user should be able to enable, disable, add and remove options from the menubar for that specific app, triggering keyboard shortcuts or running shell commands.
- When clicking in the Windows flag menu -> System Preferences... button, it should launch the System Preferences app (if you have it installed).

The functionalities that I intent to implement in the right side are:
- Showing the system tray app icons, with the right click action binded to a single click.
- Showing the Bluetooth, Wi-Fi/Ethernet, Volume, Battery, Calendar+Time and User icons with options on click.
- All the prior mentioned icons should have a Preferences option in their Menu to launch System Preferences in its specific view (if you have it installed).
- Showing a magnifying icon that will launch the Spotlight (if you have it installed).

### System Preferences
The macOS equivalent to the Windows's Control Panel is just easier to work on. The views below without a description are just intended to look as close to their macOS counterparts as possible. It should have the following views per row:
- 1st row:
   - **General**
   - **Desktop & Screen Saver**
   - **Dock**: same, but with one extra tab (Apps): to change an specific app name or icon, and to list apps that should be ignored by the Dock, other than system apps. (if you have Dock installed).
   - **Menubar**: should work as the Dock Apps tab, but for the Menubar. (if you have Menubar installed).
   - **Language & Region**
   - **Security & Privacy**: General tab only; FileVault, Firewall and Privacy should be ignored.
- 2nd row:
   - **Displays**
   - **Energy Saver**
   - **Keyboard**: for Keyboard and Input Sources only.
   - **Touchpad**: equivalent to the macOS Trackpad option.
   - **Printers & Scanners**
   - **Sound**
- 3rd row:
   - **Software Update**
   - **Network**
   - **Bluetooth**
- 4th row:
   - **Users & Groups**
   - **Date & Time**

The Dock and Menubar views should appear because their respective apps should also install a DLL that works as a plugin to the System Preferences app. 

## Ignored modules
There are things in macOS that I simply don't use (or don't use THAT much), and because of that I won't work on. In case you liked the project and want one of the modules below being a part of macOsFeel, submit a pull request and I will review it.

### Spotlight
At this moment, I just recommend you to use [Wox](https://github.com/Wox-launcher/Wox). It looks good enought (haven't tested it yet thought).

### Notification tray
Both Windows and macOS have a notification tray, but I never used it.

### Launchpad
Never used it either. 

## FAQ

### Can I change the configurations of the Dock and the Menubar without the System Preferences app?
The idea of macOsFeel is to mimic the macOS feel, so they should be configured by System Preferences, but if, for any reason, you prefer not to, their JSON config files can be edited manually. 

### Can I create my own icons and views for the System Preferences window?
Absolutely. Although, it should follow the same order of the macOS original window. So if your plugin has the name of one of the macOS System Preferences original icons, it should be in the same position that it was in macOS. In case it's an unknown plugin, it should be placed in the 5th row.
