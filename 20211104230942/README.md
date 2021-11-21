# Terminal configuration

**set -o vi** 
* **/text** to find a with specific text
* putting space(s) before command gets you into *incognito* mode. This command will not be saved in history.
* putting **\** before command removes any aliases, functions etc.
* type *command* is really cool to show where the command is (similar to which). Show aliases too.
* *stty -ixon* to disable ctrl+s shortcut (which suspend the terminal)
* custom P1 to configure command prompt
* restoring **ESC** key to its original destiny
`test -n "$DISPLAY" && setxkbmap -option caps:escape &>dev/null
* Always use *Ctrl-[* instead of *ESC*

# Background and Foreground Running Programs
* *fg* command moves job to the foreground
