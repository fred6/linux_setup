Notes for Arch Linux setup for future me's.

# Files
## /etc/bash.bashrc

This makes a simple bash prompt with color (blue), underline and absolute paths displayed

## ~/.bashrc

Same as for /etc/bash.bashrc, except the color here is purple. Used to distinguish between my user and root.


## ~/.bash_profile
Just starts X

## ~/.xinitrc

Starts the urxvtd daemon, sets keyboard to my custom layout (see below) with caps and escape swapped, enables Ctrl+Alt+Backspace to kill X, key repeat rate increased, turns off horrible deafening bell, set up desktop background, source Xresources and start xmonad.

## /usr/share/X11/xkb/symbols/carpalx

I took the carpalx X11 keyboard setup available from carpalx website and modified it by removing everything I don't use, then tweaking qwkrfy. Specifically, I use a 3-swap alternative of qwkrfy (which I've called qwkrfy3 here) which does not swap A & S or N & G. You've got to modify symbols.dir like it says, but that's straightforward.

## ~/.fehbg

feh --bg-scale '/mnt/bits/unorg/images/earthrise.jpg'

## ~/.Xresources

Major features include setting font to Terminus and setting transparency.

## ~/.xmonad/xmonad.hs

I don't know Haskell but I cobbled this together using the internet. This depends on xmonad-contrib.

##.vimrc

You also need to install the molokai theme into .vim/colors/

# Additional notes
## flash sound (youtube)
In order to get this working, have to add my username to the 'audio' group. It's required by alsa?
