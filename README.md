<img width="1920" height="1080" alt="screenshot_2026-11-19_22-27-22" src="https://github.com/user-attachments/assets/a77ac413-e7d7-470b-80e8-1573236c19a3" />
## Niri

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
sudo pacman -S --noconfirm kitty mpv eog ntfs-3g rocm-smi-lib xdg-desktop-portal-gnome adw-gtk-theme
```
