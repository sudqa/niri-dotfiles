# Arch Linux Setup

### Install `yay` (AUR Helper)
```bash
sudo pacman -S --needed git base-devel
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```
---
### Mounting HDD
```bash
sudo mkdir /mnt/hdd
sudo vim /etc/fstab
```
Add to `/etc/fstab`:
```
UUID=4ACAE882CAE86B9F  /mnt/hdd  ntfs-3g  uid=1000,gid=1000,umask=022,nofail  0  0
```
---
### Essential Packages
```bash
sudo pacman -S --noconfirm kitty mpv eog ntfs-3g rocm-smi-lib xdg-desktop-portal-gnome 
```

### Essential Themes and Fonts
```bash
sudo pacman -S noto-fonts noto-fonts-cjk noto-fonts-emoji noto-fonts-extra adw-gtk-theme
```

