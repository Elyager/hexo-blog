---
published: false
---

##Quick Tip poner simbolo unicode en la terminal

If you are on a Mac the command you want to run to put a burger in your Bash shell prompt like mine is:

    export PS1="\w 🍔  " 
	
(which will eventually end up looking like
export PS1="\w <U+1F354>  ")

CTRL + COMMAND + SPACE para sacar los simbolos

That string is \w for “current working directory”, a space, an emoji burger, and two more spaces for padding.

If you want it to be permanent put that line in your .profile or .bash_profile.

For my prompt I removed my system user name and host. People use those to know which computer they’re on and which user they are, but I know I am me and I am on the burger computer so I removed them. Here are some other options.

    \d – Current date
    \t – Current time
    \h – Host name
    # – Command number
    \u – User name
    \W – Current working directory (ie: Desktop/)
    \w – Current working directory, full path (ie: /Users/Admin/Desktop)
