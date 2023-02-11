# openbox
Debian openbox

me guie de
(La Garza Resistente)[https://www.youtube.com/watch?v=uLQTvjzd2gI]

Edit apt sources

```
sudo nano /etc/apt/sources.list
```

At the end of each url write

```
contrib non-free
```

At the bottom ad the media repository

```
# Multimedia Repo
deb http://www.deb-multimedia.org bullseye main nonfree
```

Below that

```
# Backports Repo
deb http://ftp.debian.org/debian bullseye-backports main non-free
```

Update keys and add keyring

```
sudo apt update -oAcquire::AllowInsecureRepositories=true

sudo apt install deb-multimedia-keyring
```


```
mesa-utils

nano

neofetch

htop

xorg
```
Install openbox
``` 
sudo apt install openbox obconf openbox-menu tint2 rxvt thunar nitrogen pulseaudio arandr gsimplecal picom lxpolkit firefox-esr
openbox #window manager
obconf #openbox config
openbox-menu #openbox menu autorefresh
rxvt # terminal emulator
arandr # screen resolution
pulseaudio # sytem audio
tint2 # system bar
nitrogen # wallpaper
picom # ui effects
lxpolkit # gui security policy
network-manager-gnome # internet & wifi
thunar # file manager

leafpad or litexl # text editor (need a easier option)

gsimplecal # simple calendar
galculator # calculator
firefox-esr # web browser
```
Install session manager [Ly](https://github.com/fairyglade/ly)
```
sudo apt install git
git clone --recurse-submodules https://github.com/fairyglade/ly
cd ly
make
make install installsystemd
systemctl enable ly.service
```
```
urxvt

rofi

picom

```
