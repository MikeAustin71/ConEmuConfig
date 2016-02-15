
# ConEmu Webstorm Integration
## Background
ConEmu is a Windows Terminal or Console emulator. [ConEmu](https://conemu.github.io/)

If ConEmu is configured to display Git Shell, you can in turn configure the WebStorm
'Terminal' to call ConEmu and display a Git Shell console in WebStrom's current working
directory.


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


