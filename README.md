https://github.com/user-attachments/assets/33e062df-0ef5-4445-acce-7590d82b78ce

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
UUID=???  /mnt/hdd  ntfs-3g  uid=1000,gid=1000,umask=022,nofail  0  0
```
---
### Essential Packages
```bash
sudo pacman -S --noconfirm kitty fuzzel mpv eog ntfs-3g rocm-smi-lib xdg-desktop-portal xdg-desktop-portal-wlr 
```

### Essential Themes and Fonts
```bash
sudo pacman -S noto-fonts noto-fonts-cjk noto-fonts-emoji noto-fonts-extra adw-gtk-theme
```

