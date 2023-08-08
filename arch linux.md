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
#### 安装SSH
`su`  
`pacman -Syyu`  
`pacman -S openssh`  
`systemctl start sshd`  
`systemctl enable sshd`  
`ip a`
#### 安装Aru
`nano /etc/pacman.conf`
```
Color

[archlinuxcn]
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/$arch
```
`pacman -Sy archlinuxcn-keyring`  
`pacman -S paru yay`  
#### 安装VM Tools（实体机忽略
`pacman -S gtk2 gtkmm gtkmm3 open-vm-tools xf86-video-vmware xf86-input-vmmouse`  
`systemctl enable vmtoolsd.service`  
`nano /etc/mkinitcpio.conf`  
```
MODULES=(vsock vmw_vsock_vmci_transport vmw_balloon vmw_vmci vmwgfx)
```
`mkinitcpio -p linux-zen`
#### 安装字体  
`pacman -S adobe-source-han-sans-cn-fonts adobe-source-han-serif-cn-fonts noto-fonts-cjk noto-fonts-emoji noto-fonts-extra ttf-hannom wqy-microhei wqy-zenhei`
#### 安装Fcitx5输入法
`pacman -S fcitx5-im fcitx5-chinese-addons fcitx5-material-color fcitx5-pinyin-moegirl fcitx5-pinyin-zhwiki`

**To be continued...**