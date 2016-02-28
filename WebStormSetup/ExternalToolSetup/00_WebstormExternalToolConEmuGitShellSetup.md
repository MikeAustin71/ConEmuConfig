# Configuring ConEmu Git Shell as an External Tool in Webstorm
## Background
ConEmu is a Windows Terminal emulator. [ConEmu](https://conemu.github.io/)

You can configure ConEmu to display the Git Shell. See ../../TaskConfigs/GitShell
in this directory structure.

Once Git Shell is installed as a Task (Example: {GitShell::Git Shell(Admin)},
you can configure Webstorm to call ConEmu/Git Shell as a Webstorm 'External Tool'.

## The Advantage Of Configuring ConEmu as External Tool
Once ConEmu is configured as an External Tool, you can precisely control the directory
in which ConEmu will be launched.  

Configuring ConEmu as a 'Terminal Tool' means that ConEmu will be launched in the WebStorm
Project Directory. If you have several sub-directories in your project, this means that you
will have to change directory or 'cd' to your current code directory.

Unlike the 'Terminal Setup' which launches ConEmu in the WebStorm 'Project Directory'
The External Tool configuration will launch ConEmu in the actual directory selected in
WebStorm's Project Directory tree on the left side of the screen. Add a shortcut key to
this 'External Tool' Configuration and you can quickly launch a terminal session in the
directory where you need it.


## Web External Tool Configuration
For setup details see the images in this directory
* 01_WebstormExternalToolConEmuConfig.jpg
* 02_WebstormExternalToolConEmuConfig.jpg

## Configure ShortCut Key for ConEmu External Tool
The icing on the cake in terms of productivity is to configure a shortcut
key for the ConEmu 'External Tool'. The short cut key is configured in
WebStorm 'Settings' view as shown in the following image files in this
directory:
* ConfigExternalToolShortCutKey_01.jpg
* ConfigExternalToolShortCutKey_02.jpg
* ConfigExternalToolShortCutKey_03.jpg
