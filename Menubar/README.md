# macOsFeel Menubar
The macOS menubar can't be perfectly recreated in Windows since the menubar of Windows application is inside their own windows, but that doesn't mean we can't have a menubar. The functionalities that I intent to implement in the left side are:
- Showing a Windows flag menu (for the same system-related options found in the macOS's Apple menu).
- Showing the app name menu, with the common options: About, Preferences..., Hide App, Hide Others, Show All, Quit App.
- Showing the Window menu, with the common options.
- When clicking in the app name menu -> Preferences... button, the user should be able to enable, disable, add and remove options from the menubar for that specific app, triggering keyboard shortcuts or running shell commands.
- When clicking in the Windows flag menu -> System Preferences... button, it should launch the System Preferences app (if you have it installed; otherwise it should launch Windows's Control Panel).

The functionalities that I intent to implement in the right side are:
- Showing the system tray app icons, with the right click action binded to a single click.
- Showing the Bluetooth, Wi-Fi/Ethernet, Volume, Battery, Calendar+Time and User icons with options on click.
- All the prior mentioned icons should have a Preferences option in their Menu to launch System Preferences in its specific view (if you have it installed; otherwise it should launch its Windows's Control Panel counterpart).
- Showing a magnifying icon that can run a shell command (to launch the Spotlight, if you have it installed).
