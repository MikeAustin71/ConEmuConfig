# ConEmu Task Configurations
ConEmu is a free Terminal Emulator for windows.  This configuration information is taken from my Window 10 machine.

Installing a terminal emulator like ConEmu will allow one to seamlessly integrate the command terminal with WebStorm and Git Shell. This makes it easy to navigate directories when building golang projects on Windows.

## Background
ConEmu is a free Windows Terminal\Console emulator. [ConEmu](https://conemu.github.io/)

ConEmu consoles can be configured to display various utilities such as PowerShell,
Windows Command Prompt and Git Shell.

If you use WebStorm, ConEnmu can be configured as an 'External Tool' or 'Terminal'
which can then be called from the Webstorm IDE displaying WebStorm's current working directory.
I like the 'External Tool' configuration because you can call it from the Project Tree in Webstorm
and specify the precise directory where you want to launch the terminal emulator. No changing
directories required.

The information in the 'TaskConfigs' folder shows how to configure ConEmu 'Tasks'.  If you are not
familiar with the 'Tasks' concept, review the docs for ConEmu.

The information in the 'WebStormSetup' folder shows how to configure WebStorm to call ConEmu
from within the WebStorm IDE.

# If you choose NOT to use a Terminal Emulator (ConEmu)
* You can configure Git Shell in Webstorm using the path to the Git Shell executable.
* The Git Shell executable is installed on my Windows 10 machine in directory:
    ```
    C:\Users\yourusername\AppData\Local\GitHub\PortableGit_c7e0cbde92ba565cb218a521411d0e854079a28c
    ```
* The Git Shell executable, 'git-bash.exe', is stored in this 'user' directory created by the install program.

## Git Shell - How To Clear The Console

* Note: Git Shell Installation (the actual executable) is located under 'GitHub' directory
    1. Example: C:\Users\yourusername\AppData\Local\GitHub\PortableGit_c7e0cbde92ba565cb218a521411d0e854079a28c
    * git-bash.exe is stored in this 'user' directory created by the install program.

* __How to clear the console window__
    1. Look inn 'etc' directory C:\Users\yourusername\AppData\Local\GitHub\PortableGit_c7e0cbde92ba565cb218a521411d0e854079a28c\etc
    * Find the file: bash.bashrc
    * Add these alias lines at the bottom of the bash.bashrc file:
            ```
            # Clear Alias
            alias clear='printf "\033c"'
            alias cls='printf "\033c"'
            ```
    * After these alias parameters are configured, simply type 'cls' or 'clear' at the command window
      to clear the console window.
    * On my Windows 10 machine Ctrl+L will also clear the console.

## Launch Windows Explorer From Terminal Console
    * Launch Windows Explorer from the console. Explorer will default to the current directory.
    * In Git Shell execute: "start . <ENTER>"
    * "start . <ENTER>" works in the Git Shell without ConEmu.
