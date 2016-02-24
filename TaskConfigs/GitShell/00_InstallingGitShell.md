# Terminal Emulator - Git Shell
* Git Shell is a terminal emulator
* It allows use of linux commands from a Windows machine
*

## Github Desktop

### Github Desktop Contains Git Shell
* You can find Github Desktop here:
* Some say don't open in Chrome. I didn't have a problem.
* https://desktop.github.com/
* Git Shell is part of Github Desktop

### Github Desktop Configuration Procedure
##   Get The Terminal Emulator
1. [Open in anything except Chrome](https://desktop.github.com/)
* Under Title: 'Find Simple collaboration from your desktop'
* Click Button 'Download GitHub Desktop'
* Install
* Under Settings/Options Set Shell = 'Git Bash'
* Use Git Bash
* open it and test it
* basic terminal commands
    * ls
        * ls -la
    * cd
    * cd ../
    * pwd


## Git Shell
1. Shell Command
    * C:\Users\yourusername\AppData\Local\GitHub\GitHub.appref-ms --open-shell

* Shortcut Location
    * C:\Users\yourusername\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\GitHub, Inc

* Note: Git Shell Instllation (the actual executable) is located under 'GitHub' directory
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

## Use Basic Unix Terminal Commands
[How to Use Basic UNIX Commands](http://www.dummies.com/how-to/content/how-to-use-basic-unix-commands-to-work-in-terminal.html)
* pwd = print working directory
* ls -la  (List Directory Contents)
