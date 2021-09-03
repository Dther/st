# Dther's Simple Terminal Fork
A personal fork of the suckless st (simple terminal). 

The main important part of this repository is config.h, but
future patches may be added for functionality's sake.

## Current Planned Patches
   * iso14755
   * Some kind of prompt to prevent accidental quitting by X
    
## Patches that were added at one point, but later removed
   * alpha
        * Could be accomplished by modifying compton.conf.
   * scrollback
        * Could be accomplished with tmux, with the added benefit of
            everything tmux provides.
   * Xresources
        * Consistent colours are good for syntax highlighting, wal
            colour schemes have unfortunately poor contrast.

Original README
--------------------
st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

