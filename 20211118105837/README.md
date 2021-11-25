# Scripting in POSIX Shell

* **POSIX** -> Portable Operation System Interface
* you can see things about a process with *cd number_of_a_process* for eg. cd 34958 (virtual filesystem). There you can see:
 * what is running -> *ls -l exe*
 * where the file of this process is placed -> *ls -l cwd*
 * what is the name of a command -> *cat cmdline*
* add `#!/bin/sh` shebang line to specify interpreter (#!/usr/bin/python3 should work as well)
* **NEVER** use `./` in your PATH 
* Functions vs Procedures
 * Function has a return, procedure not necessarily
 * Function is like a black box, you put stuff in, you get stuff out. It is self-contained. Procedure works out of its scope.
* use shellcheck on scripts for static analysis
* single quotes (' ') puts variable extensions off 
* add `set -e` at the beginning of the script to ensure program exits if **anything** fails. Also show debug steps.
* POSIX doesnt have switches (options) on echo:
 * echo -e hello -> -e hello
 * #!/bin/bash -> echo -e hello -> hello
* **I WILL ALWAYS QUOTE MY VARIABLES WITH CURLY BRACKETS IN SHELL** "${variable}"
* use bc when math and numbers are needed 
* *Parameters are to arguments as variables are to values*
* every variable in POSIX is global (*local works* but its not POSIX)

## Function and Command Communication

* calls must be done after declaration
* cd 'workspace d' -> but prefer to use $() over backticks, just for nesting.
* use `$#` to get the total number of arguments passed
* use `$@` for `first` `second` `third`
* use `$*` for `first second third`
* use `$?` for last return value
* Shell functions only returns integers
 * use return [RVALUE] to set return value
 * omitting return is fine
 * return values are not output


