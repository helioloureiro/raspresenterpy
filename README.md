Raspberry Presenter
===================


It is a lightweight system to present in raspberrypies
in kiosk mode.  The intent is to have a way to
display several jenkins outputs (or similar).

Written in python (it workins in 2.6 and above) and
python Qt (Qt4).

And using WebKit.

Thanks for Gustavo Noronha for challenge me to create
that.

Note
====

I found a bug in raspberrypi implementation of libqt
and webkit on Wheezy version (raspbian).  It was 
linked against old libwebkitgtk-1 instead
libwebkitgtk-3.

On recently released Jessie, it is working just fine.

Limitations
===========

There is a memory leak in some place that I couldn't
find and get rid off.  So... sadly I need to "kill"
the presenter from times to times.  I'm including a
shell script to bring it up again but... yap, far 
from good.
