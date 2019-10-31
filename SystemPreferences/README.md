# macOsFeel System Preferences
The macOS equivalent to the Windows's Control Panel is just easier to work on. The views below without a description are just intended to look as close to their macOS counterparts as possible. It should have the following views per row:
- 1st row:
   - **General**
   - **Desktop & Screen Saver**
   - **Dock**: same, but with one extra tab (Apps): to change an specific app name or icon, and to list apps that should be ignored by the Dock, other than system apps (the app may be ignored from the Applications view, or from the opened apps group). (if you have Dock installed).
   - **Menubar**: with two tabs: General and Apps. Apps should work as the Dock Apps tab, but for the Menubar. General should allow you to enable/disable any of its default icons, binding shell commands to them or leaving them with their default actions (if you have Menubar installed).
   - **Language & Region**
   - **Security & Privacy**: General tab only; FileVault, Firewall and Privacy should be ignored.
- 2nd row:
   - **Displays**
   - **Energy Saver**
   - **Keyboard**: for Keyboard and Input Sources only.
   - **Mouse**
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

May start using the [Ultimate Settings Panel](https://github.com/techygeekshome/Ultimate-Settings-Panel) source.
