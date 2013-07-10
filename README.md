dwm 6.0
=======

requirements
------------

 * [dmenu](http://tools.suckless.org/dmenu/)(using in dclip)
 * [slock](http://tools.suckless.org/slock)(optional, config.h keys)
 * [skb](https://github.com/polachok/skb)(using in status script)

installation
------------

```bash
cd ~/sft/
git clone git@github.com:qbbr/dwm.git
cd dwm/
patch -p1 < dwm-6.0-statuscolors.diff
patch -p1 < dwm-6.0-gaplessgrid.diff
patch -p1 < dwm-6.0-marginbottom.diff
cp config.h.dist config.h
sudo make install clean
sudo ln -s ~/sft/dwm/sft/dclip /usr/bin/
```

add to .xinitrc

```bash
~/sft/dwm/bin/startdwm
```

overview
--------

available patches:

 * [gapless grid](http://dwm.suckless.org/patches/gapless_grid)
 * [gridmode](http://dwm.suckless.org/patches/gridmode)
 * [statuscolor](http://dwm.suckless.org/patches/statuscolors)
 * [ansistatuscolors](http://dwm.suckless.org/patches/ansistatuscolors)
 * marginbottom

enabled patches:

 * gapless grid
 * statuscolor
 * marginbottom

hotkeys:

 * [Ctrl] + [Mod] + [c] = copy to clipboad (dclip)
 * [Ctrl] + [Mod] + [v] = paste to clipboad, using dmenu (dclip)
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

 * ![dwm statuscolor skb en](https://lh5.googleusercontent.com/-4EfhPoZZKGM/TnEtZlFRbbI/AAAAAAAAAdU/NqZk9BEi_7c/s800/dwm-statuscolor-skb-en.png "skb en")
 * ![dwm statuscolor skb ru](https://lh4.googleusercontent.com/-CuqeTPkzz6Y/TnEtZgi4CbI/AAAAAAAAAdY/v1isBwqx3YU/s800/dwm-statuscolor-skb-ru.png "skb ru")
