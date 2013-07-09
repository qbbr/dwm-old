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
cp config.h.dist config.h
sudo make install clean
sudo ln -s ~/sft/dwm/dclip /usr/bin/
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

statuscolor with skb:

 * ![dwm statuscolor skb en](https://lh5.googleusercontent.com/-4EfhPoZZKGM/TnEtZlFRbbI/AAAAAAAAAdU/NqZk9BEi_7c/s800/dwm-statuscolor-skb-en.png "skb en")
 * ![dwm statuscolor skb ru](https://lh4.googleusercontent.com/-CuqeTPkzz6Y/TnEtZgi4CbI/AAAAAAAAAdY/v1isBwqx3YU/s800/dwm-statuscolor-skb-ru.png "skb ru")
