# openbox
Debian openbox

me guie de
(La Garza Resistente)[https://www.youtube.com/watch?v=uLQTvjzd2gI]

# Edit apt sources

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

openbox

urxvt

rofi

picom

```
