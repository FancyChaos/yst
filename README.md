# yst - st patched

**yst** is a version of [st](https://st.suckless.org/) with some suckless patches already applied to it.

The compiled executable will still be named **st**.

## Included patches

- [autocomplete](https://st.suckless.org/patches/autocomplete/)
- [scrollback](https://st.suckless.org/patches/scrollback/)
- [alpha](https://st.suckless.org/patches/alpha/)
- [ligatures](https://st.suckless.org/patches/ligatures/)
- [blinking cursor](https://st.suckless.org/patches/blinking_cursor/)
- [spoiler](https://st.suckless.org/patches/spoiler/)
- [vertcenter](https://st.suckless.org/patches/vertcenter/)
- [delkey](https://st.suckless.org/patches/delkey/)
- [w3m](https://st.suckless.org/patches/w3m/)
- [Xresources](https://st.suckless.org/patches/xresources/)

## Additional patches

Additional patches can be applied by sourself.
I use them for my automated install scripts.

- fontsize28 (Own patch to increase the font size to 28)
- [openbsd](https://st.suckless.org/patches/openbsd/)

## Note

*config.mk.openbsd* includes the libraries and for flags OpenBSD.
Rename that file to *config.mk* to compile for OpenBSD.

*Fire Code Nerd Font* is required (Or just change the font yourself).

------------

## Original README

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


