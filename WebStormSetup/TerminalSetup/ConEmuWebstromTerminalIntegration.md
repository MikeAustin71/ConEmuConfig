
# ConEmu Webstorm Integration
## Background
ConEmu is a Windows Terminal or Console emulator. [ConEmu](https://conemu.github.io/)

If ConEmu is configured to display Git Shell, you can in turn configure the WebStorm
'Terminal' to call ConEmu and display a Git Shell console in WebStrom's current working
directory.

To see a sample 'Terminal' configuration in WebStorm, reference the image file in this directory:

* 01_WebStormTerminalConfiguredForConEmuGitShell.jpg

## Considerations
Configuring ConEmu as00_WebstormExternalToolConEmuGitShellSetup 'Terminal' Tool means that when activated, ConEmum will be launched in the
WebStorm 'Project Directory'.  If you have several sub-directories in your project, this means
that you will have to change directory or 'cd' to your current code directory.

As an alternative, you could configure ConEmu as an 'External Tool' which will allows to specify the target
directory in the WebStorm Project Tree View where ConEmu will be launched.
* __../ExternalToolSetup/00_WebstormExternalToolConEmuGitShellSetup.md__

## Example of Simple WebStorm Terminal Config Using ConEmu
__This is a simple configuration which displays the 'default' ConEmu Task__

[Simple ConEmu Setup](https://cloud.githubusercontent.com/assets/7850073/7632984/fe3fe434-fa59-11e4-85c7-499dd5675c86.png)


## Example of WebStorm Terminal Configured for Git Shell in ConEmu
__This procedure configures the WebStorm Terminal to display the Git Shell in ConEmu.__

* 1. See 01_WebStormTerminalConfiguredForConEmuGitShell.jpg in this directory.
* Note: You will first need to configure the ConEmu Git Shell Task named '{GitShell::Git Shell(Admin)}'
    * See ../TaskConfigs/GitShell for ConEmu Git Shell Configuration
* Terminal Configuration Syntax:
```
C:\Program Files\ConEmu\ConEmu64.exe -cmd {GitShell::Git Shell(Admin)}
```
