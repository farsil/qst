#qst - quasi simple terminal
qst is a modified version of [st](http://st.suckless.org), the simple terminal
emulator for X which sucks less. Compared to plain st it has scrollback 
support and rxvt's intensityStyles option emulation.

#Requirements
No other requirements rather than the Xlib header files, as in regular st.

#Installation
Edit config.mk to match your local setup (st is installed into
the `/usr/local` namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install

#Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -s st.info

See the man page for additional details.

#Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
Scrollback implementation inspired by the official upstream patch.
