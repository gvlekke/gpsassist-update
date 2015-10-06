The goal of this project is to provide OS X users with a tool to automatically update the GPSAssist-data on their Sony GPS-enabled camera (DSC-HX5V).
Sony currently does not provide software for OS X to update the GPSAssist-data.

  1. Download the GPSAssist Update 1.0.1.zip from Downloads
  1. Unzip it and drag to your Applications
  1. Run it and it should all be pretty clear (i hope)
  1. If you want to run it automatically at startup add it to your Login-items in the System Preferences -> Accounts

This is just a small utility that monitors mounted filesystems. If a filesystem contains a Private/SONY directory the user is prompted if the GPSAssist-data on this disk should be automatically updated. The data is updated once every 24 hours. The application is running as a background-application. You can access it via the GPS-icon in the status-menu on top of the screen.

You might want to set the LUN-settings in your camera to Single. This way only the storage-card is mounted, not the internal memory (which has label NO NAME and cannot be changed afaik).

If you have installed Growl (and why not?) you will get notifications of the update of GPSAssist-data.

Settings for each disk are stored in a .gpsassist.plist-file in the root of that disk.

Use this tool at your own risk.
Do whatever you want with the code, i just created it to do some OS X programming (after a lot of iPhone programming). And i wanted to try Growl :)

If you are having problems or need more features create a new "issue" here. I may find some time to fix it.