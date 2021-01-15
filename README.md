st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.

*my own fork which contains some customization, here is the main repo https://git.suckless.org/st/file/README.html*
+ kitty mathias theme ([https://github.com/dexpota/kitty-themes/blob/master/themes/Mathias.conf](https://github.com/dexpota/kitty-themes/blob/master/themes/Mathias.conf))
+ scrollback patch (shift + (pageup/pagedown)) [scrollback](https://st.suckless.org/patches/scrollback/)
+ boxdraw patch [boxdraw](https://st.suckless.org/patches/boxdraw/)

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

