## Ubuntu[18.04] 
#### 1.Set Mouse Speed
```sh
xinput --list
xinput --list-props [device id]
xinput --set-prop [device id] [value]
sudo vim /ect/profile.d/mouse.sh
    [set mouse commond]
```
### 2.Wifi Adapter RTL8812AU
```sh
lsusb [-v]
sudo modprobe -a rtl8812au
```

### 3.Fix Time
```sh
sudo apt-get install ntpdate
ntpdate cn.pool.ntp.org
date 
timedatectl
```

### 4.
```sh
sudo passwd
sudo apt install ibus-pinyin
sudo apt install tmux
sudo apt install zsh //ohmyzsh
```