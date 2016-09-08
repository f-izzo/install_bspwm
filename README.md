# Install bspwm
## What this script does:
- install the dependencies
- compile __bspwm__, __sxhkd__, __lemonbar__ 
- install the above programs
- configure environment variables and copy example configurations.

The dependecies installation should work on __Fedora__, __Ubuntu__ and __Arch__, however i have tested only Fedora, so please open an issue or pull request if you find missing dependencies.
### Notes
__This installation requires a working display manager like GDM, KDM, LightDM__
To avoid using a Display Manager you can append the following to your ~/.xinitrc `exec bspwm`

## Usage
Clone this repository and execute `./install_bspwm`, reboot and select _bspwm_ from the session list.

## To uninstall
Uninstallation is not yet implemented, you can do the following:
- Go into `install_bspwm/build`, enter each subfolder and issue `sudo make uninstall`
- Delete `.config/bspwm` and `.config/sxhkd`
- Remove the last lines from `~/.bash_profile`
- Delete `bspwm.desktop` from `/usr/share/xsessions/`
- You can also remove the dependencies listed in the script

#### Credits
[Windelicato's bspwm guide](https://github.com/windelicato/dotfiles/wiki/bspwm-for-dummies)
