# Matrix-GrubTheme
Matrix theme for Grub2 bootloader 
## Installation
1. Clone repository into `/boot/grub/themes` directory (or wherever your GRUB installation resides):
```
sudo mkdir -p /boot/grub/themes && cd /boot/grub/themes
sudo git clone https://github.com/Feasuro/Matrix-GrubTheme.git
```
2. Change theme setting in `/etc/default/grub` file:
```
sudo sed -i '/^GRUB_THEME=/d' /etc/default/grub
printf '\nGRUB_THEME=/boot/grub/themes/Matrix-GrubTheme/theme.txt\n' | sudo tee -a /etc/default/grub
```
3. Rebuild your GRUB configuration:

`sudo update-grub` or `sudo grub-mkconfig -o /boot/grub/grug.cfg`
____________________________________________________________________________
Created by [Feasuro](https://github.com/Feasuro)
