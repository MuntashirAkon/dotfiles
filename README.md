# The Voidrice

**NOTE:** This repo doesn't strictly follow LARBS (shortcut's are still kept the same/similar). My preferred WM is `bspwm` and status bar is `polybar`.

Additionl Prerequisites:
- (AUR) polybar (Optional, if you want to use bspwm)
- bspwm (Optional)
- zzz (Optional, comes default with runit systems, without it sleep and hibernate won't work)
- rofi (dmenu replacement)
- (AUR) rofi-dmenu (dmenu compatibility)
- xss-lock
- xorg-appres (x11-utils for debian) (Optional, for changing dunst theme based on current Xresources). To convert your current `dunstrc`, run the following:
  ```sh
  dunst_xr_theme_changer.sh && mv -f ~/.config/dunst/dunstrc{_xr_colors,}
  ```
- picom (you can remove xcompmgr)
- pulseaudio (`amixer` is still used for volume control)
- (AUR) pulseaudio-alsa

Other changes:
- Themes can be added (located at `~/.colors`) at `~/.Xresources` (current theme is `empire`)
- Some additional shortcuts added (see at `~/.config/sxhkd/sxhkdrc`)

And don't be a fool and replace the crappy (Chromium based) Brave browser with hardened Firefox.

**By the original author**

These are the dotfiles deployed by [LARBS](https://larbs.xyz) and as seen on [my YouTube channel](https://youtube.com/c/lukesmithxyz).

- Very useful scripts are in `~/.local/bin/`
- Settings for:
	- vim/nvim (text editor)
	- zsh (shell)
	- i3wm/i3-gaps (window manager)
	- i3blocks (status bar)
	- sxhkd (general key binder)
	- ranger (file manager)
	- lf (file manager)
	- mpd/ncmpcpp (music)
	- sxiv (image/gif viewer)
	- mpv (video player)
	- calcurse (calendar program)
	- tmux
	- other stuff like xdg default programs, inputrc and more, etc.
- I try to minimize what's directly in `~` so:
	- All configs that can be in `~/.config/` are.
	- Some environmental variables have been set in `~/.zprofile` to move configs into `~/.config/`
- Bookmarks in text files used by various scripts (like `~/.local/bin/shortcuts`)
	- File bookmarks in `~/.config/files`
	- Directory bookmarks in `~/.config/directories`

## Want even more?

My setup is pretty modular nowadays.
I use several suckless programs that are meant to be configured and compiled by the user and I also have separate repos for some other things.
Check out their links:

- [dwm](https://github.com/lukesmithxyz/dwm) (the window manager I usually use now which is fully compatible with this repo)
- [st](https://github.com/lukesmithxyz/st) (the terminal emulator assumed to be used by these dotfiles)
- [mutt-wizard (`mw`)](https://github.com/lukesmithxyz/mutt-wizard) - (a terminal-based email system that can store your mail offline without effort)

## Install these dotfiles

Use [LARBS](https://larbs.xyz) to autoinstall everything:

```
curl -LO larbs.xyz/larbs.sh
```

or clone the repo files directly to your home directory and install [the prerequisite programs](https://github.com/LukeSmithxyz/LARBS/blob/master/progs.csv) or [those required for the i3 setup](https://github.com/LukeSmithxyz/LARBS/blob/master/legacy.csv).
