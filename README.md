# Bodhi-Update

Bodhi-Update is a fork of rdum - riban's dpkg update monitor

This simple shell script provides an indication of available updates on a dpkg / apt system. It shows status with an icon in the system tray which indicates if any updates are available and whether any are security updates. The system tray icon tooltip shows how many updates are available.

Left click on the system tray icon will open a dialog showing a list of available updates and offer to install them.

Right clicking on the system tray icon shows a menu allowing:
* Check for new updates
* Show list of available updates (and offer to install them - same as left click on icon)
* Install all available updates
* Refresh the status of the system tray icon (in case background check has found updates)
* Quit the update monitor

The icon refreshes its status every 10 minutes but depends on a background task to check for new updates automatically. Status is also refreshed after triggering any action from the system tray icon. Whilst refresh is occuring the application ignores commands.

Depends on:
* yad - Provides the system tray interface
* xterm - Displays apt commands
* awk - Decoding, etc.
* bash - This is a bash script
* apt - Get update status
* apt-get - Performs updates and upgrades


