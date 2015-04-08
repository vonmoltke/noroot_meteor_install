Fork of the Meteor install script that doesn't need root or sudo.

I created this script after trying to install Meteor on systems where I do not have sudo permissions or root access.  This version of the script does a local install by creating directories in $HOME and adding those directories to the user's $PATH.

This version also uses a symlink for getting the Meteor CLI on the user's path.  This means the target called does not need to be updated every time Meteor is updated.  Thus, a user can manually put the link in a protected system path and not need to worry about root access in the future.

Note that I have provided no easy means of doing "curl $SCRIPT | sh".  I hate that insecure anti-pattern and will not facilitate it.

