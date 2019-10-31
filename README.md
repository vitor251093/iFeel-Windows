# macOsFeel (Windows)
\[WIP\] Scripts and Apps to mimic the macOS Mojave feel in Windows 10

**WARNING: None of the stuff mentioned below was done yet. Consider this as the plans for a new project**

## Modules
macOsFeel tries to mimic the macOS appearance and functionalities, but each part of it is an individual app or script, and they are not dependent of each other. Here, you can check the created modules names:

- Dock
- Menubar
- System Preferences

Be warned: this is being created for personal use, focusing in my macOS experience, and the features that I would miss the most while migrating to a Windows computer. In case you miss anything, submit a pull request with the change.

### Future modules
Those modules are apps that I like in macOS, but which I have no plans to recreate in Windows yet because the alternatives are not that bad. The may be done in the future, but they are not my top priority.

#### TextEdit
Basically Wordpad and Notepad combinated into a single app, but with a cleaner UI.

#### Finder
For now, the Windows Explorer will do just good, but it would be interesting to recreate the Finder look in Windows in the future, since it has a more simple UI.

### Ignored modules
There are things in macOS that I simply don't use (or don't use THAT much), and because of that I won't work on. In case you liked the project and want one of the modules below being a part of macOsFeel, submit a pull request and I will review it.

#### Calendar
I love the macOS Calendar, but the Windows 10 calendar seems to be just good enought. Haven't tested it yet thought.

#### Calculator
Same as above. macOS has a nice Calculator, but Windows 10 also does. There is no need to work on replicating it.

#### Spotlight
At this moment, I just recommend you to use [Wox](https://github.com/Wox-launcher/Wox). It looks good enought (haven't tested it yet thought).

#### Notification tray
Both Windows and macOS have a notification tray, but I never used it.

#### Launchpad
Never used it either. 

## FAQ

### Can I change the configurations of the Dock and the Menubar without the System Preferences app?
The idea of macOsFeel is to mimic the macOS feel, so they should be configured by System Preferences, but if, for any reason, you prefer not to, their JSON config files can be edited manually. 

### Can I create my own icons and views for the System Preferences window?
Absolutely. Although, it should follow the same order of the macOS original window. So if your plugin has the name of one of the macOS System Preferences original icons, it should be in the same position that it was in macOS. In case it's an unknown plugin, it should be placed in the 5th row.
