dwm 6.1
=======

see also [dzenbar](https://github.com/qbbr/dzenbar)

requirements
------------

 * [dmenu](http://tools.suckless.org/dmenu/)(using in dclip)
 * [slock](http://tools.suckless.org/slock)(optional, config.h keys)
 * [skb](https://github.com/polachok/skb)(using in status script)

installation
------------

```bash
cd ~/sft/
git clone https://github.com/qbbr/dwm.git
cd dwm/
patch -p1 < dwm-6.1-statuscolors.diff
patch -p1 < dwm-6.1-systray.diff
patch -p1 < dwm-6.1-gaplessgrid.diff
patch -p1 < dwm-6.1-bottommargin.diff
cp config.h.dist config.h
sudo make install clean
```

add to .xinitrc

```bash
~/sft/dwm/bin/startdwm
```

overview
--------

available patches:

 * [statuscolor](http://dwm.suckless.org/patches/statuscolors)
 * [systray](http://dwm.suckless.org/patches/systray)
 * [gapless grid](http://dwm.suckless.org/patches/gapless_grid)
 * [bottommargin](http://dwm.suckless.org/patches/bottommargin)

hotkeys:

 * [Mod] + [Ctrl] + [c] = copy to clipboad (dclip)
 * [Mod] + [Ctrl] + [v] = paste to clipboad, using dmenu (dclip)
 * [Ctrl] + [Pause]     = lock screen (slock)
 * [Ctrl] + [PrtScr]    = take screenshot (scrot)
 * [Ctrl] + [Num /]     = volume down (volumechanger)
 * [Ctrl] + [Num *]     = volume up (volumechanger)
 * [Ctrl] + [Num -]     = volume mute/unmute (volumechanger)
 * [Ctrl] + [Num +]     = switch Headphone <-> Front output
 * [Ctrl] + [Num 5]     = mpd pause/play (mpc)
 * [Ctrl] + [Num 4]     = mpd previous track (mpc)
 * [Ctrl] + [Num 6]     = mpd next track (mpc)
 * [Ctrl] + [Num 7]     = mpd seek backward (mpc)
 * [Ctrl] + [Num 9]     = mpd seek forward (mpc)

statuscolor with skb:

 * ![dwm statuscolor skb en](https://lh5.googleusercontent.com/-lx-o5t1wLts/Udz_wejFaZI/AAAAAAAABHo/v7yQ6cP8pbU/w350-h18-no/dwm-status-en.png "dwm status skb en")
 * ![dwm statuscolor skb ru](https://lh3.googleusercontent.com/-XXU_byQ7YmY/Udz_wc2BbCI/AAAAAAAABHk/2hXM56vy9iE/w350-h18-no/dwm-status-ru.png "dwm status skb ru")
