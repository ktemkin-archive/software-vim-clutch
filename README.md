Software VIM-Clutch for Linux
===============================================================

Inspired by Aleksandr Levchuk's [VIM Clutch]{https://github.com/alevchuk/vim-clutch#readme}, this project allows you to use a hardware pedal to enter and exit VI's insert mode. Unlike the original VIM-Clutch, this software-based implementation requires no modification to the hardware pedal- and thus is only half the price!

System Requirements
======================

Software:

- A modern version of Linux, with a kernel greater than 2.6.35, and/or the uinput module. This should be most linux users.
- A modern version of X, set up to use evdev. Again, this should be almost everyone.
- Python 2.7
- The following python modules:
-- evdev
-- asyncore

Hardware:

- A USB Human Interface Device (HID) foot pedal, like [this one]{http://www.pcsensor.com/index.php?_a=viewProd&productId=2}. Any HID pedal should work, though you'll need to modify a line 

Setup/Use
==========================

Before you begin, you'll need to perform a one-time setup for your pedal. This process is two-fold:

1. Find and install the configuration software that came with your pedal. If you're using the pedal linked above, [the official Windows software is located here]{http://www.pcsensor.com/uploadFile/APPsoftware/FootSwitch%20V5.0.zip}. If you're using a Linux or Mac PC, you can perform this first step using an unsupported [command line tool]{https://github.com/rgerganov/footswitch}. 
2. Set the pedal to send *only* a chording key. Ctrl, Alt, Shift, and Windows/Super are all valid chording keys- it doesn't matter which ones you pick. If you're setting up more than one pedal, it helps to assign a different key to each pedal- this makes configuration easier.


