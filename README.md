# Rawley's fork of dwm
This is my customized fork of (dwm)[https://dwm.suckless.org]. Its lightly patched, and contains the just the necessities.
If you're looking to use this fork please check out my fork of (st)[https://github.com/rawleyfowler/st] for the best experience.

Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.

About

My customized fork of dwm.
Topics
window-manager
Resources
Readme
License
MIT license
Stars
1 star
Watchers
1 watching
Forks
1 fork
Contributors 14

    @garbeam
    @hiltjo
    @cls
    @rawleyfowler
    @anydot
    @cdown
    @schachmat
    @ericpruitt
    @dcousens
    @ianremmler
    @bakkeby

+ 3 contributors
Languages

C 91.9%
Roff 5.7%
Makefile 2.3%
Shell 0.1%
