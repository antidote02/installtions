## Arch Linux入门
**官网：https://archlinux.org/**  
**维基：https://wiki.archlinuxcn.org/wiki/%E9%A6%96%E9%A1%B5**
#### **下载Arch Linux**
https://mirrors.tuna.tsinghua.edu.cn/archlinux/iso/
#### **安装Arch Linux**
`archinstall`
#### 重启Arch Linux
`exit`  
`reboot`
#### 本地化
`su`  
`pacman -Syyu`  
`timedatectl set-timezone 'Asia/Shanghai'`  
`timedatectl set-ntp true`    
`nano /etc/pacman.conf`
```
Color

[archlinuxcn]
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/$arch
```
`pacman -Sy archlinuxcn-keyring`  
`pacman -S yay`  
* 字体  
`pacman -S adobe-source-han-sans-cn-fonts`  
`pacman -S adobe-source-han-serif-cn-fonts`  
`pacman -S noto-fonts-cjk`  
`pacman -S noto-fonts-emoji`  
`pacman -S noto-fonts-extra`  
`pacman -S ttf-hannom`  
`pacman -S wqy-microhei`  
`pacman -S wqy-zenhei`  
  * 或  
`pacman -S adobe-source-han-sans-cn-fonts adobe-source-han-serif-cn-fonts noto-fonts-cjk noto-fonts-emoji noto-fonts-extra ttf-hannom wqy-microhei wqy-zenhei`

**To be continued...**