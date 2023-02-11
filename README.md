# openbox
Debian openbox

me guie de
[La Garza Resistente](https://www.youtube.com/watch?v=uLQTvjzd2gI)

Edit apt sources

```
sudo nano /etc/apt/sources.list
```

At the end of each url write

```
contrib non-free
```

At the bottom add the media & backports repo

```
# Multimedia Repo
deb http://www.deb-multimedia.org bullseye main nonfree

# Backports Repo
deb http://ftp.debian.org/debian bullseye-backports main non-free
```

Update keys and add keyring

```
sudo apt update -oAcquire::AllowInsecureRepositories=true

sudo apt install deb-multimedia-keyring
```
Firmware problems? check [debian guide](https://www.debian.org/releases/bullseye/i386/ch06s04.en.html)

```
firmware-linux

mesa-utils

nano

neofetch

htop

xorg
```
Install openbox
``` 
sudo apt install openbox obconf openbox-menu tint2 rxvt thunar nitrogen pulseaudio arandr gsimplecal picom lxpolkit firefox-esr
```
```
openbox #window manager
obconf #openbox config
openbox-menu #openbox menu autorefresh
rxvt # terminal emulator
arandr # screen resolution
pulseaudio # sytem audio
pnmixer # audio volume
tint2 # system bar
nitrogen # wallpaper
picom # ui effects
lxpolkit # gui security policy
network-manager-gnome # internet & wifi
thunar # file manager
thunar-archive-plugin #
lxappearance # lxde theme switcher
xarchiver # archive manager
p7zip-full p7zip-rar rar unrar unzip unace bzip2 # archive format

leafpad or litexl # text editor (need a easier option)

gsimplecal # simple calendar
galculator # calculator
feh or eog # image viewer
firefox-esr # web browser
```
Install session manager [Ly](https://github.com/fairyglade/ly)
```
sudo apt install build-essential libpam0g-dev libxcb-util-dev git
git clone --recurse-submodules https://github.com/fairyglade/ly
cd ly
make
sudo make install installsystemd
sudo systemctl enable ly
```
```
urxvt

rofi

picom

```
