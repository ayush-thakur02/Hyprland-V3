# Hyprland v3
![Hyprland](https://repository-images.githubusercontent.com/470730648/c4c69fe5-dc70-42b8-aae1-3a6d303656c0)

This is version 3 of the Hyprland install script collection, which includes dot config files for hyprland as well as a basic install script for a new Arch linux installation with yes.

With this command, you may manually download the configuration files and install programmes.

**Do this ONLY if you need Nvidia support (do this first)**
```
yay -S linux-headers nvidia-dkms qt5-wayland qt5ct libva libva-nvidia-driver-git

Add modules: nvidia nvidia_modeset nvidia_uvm nvidia_drm to /etc/mkinitcpio.conf

Generate new image: sudo mkinitcpio --config /etc/mkinitcpio.conf --generate /boot/initramfs-custom.img

Add/create the following: options nvidia-drm modeset=1 in /etc/modprobe.d/nvidia.conf

reboot!
```

**Now install the below for Hyprland**

```
yay -S hyprland kitty jq mako waybar-hyprland swww swaylock-effects \
wofi wlogout xdg-desktop-portal-hyprland swappy grim slurp thunar \
polkit-gnome python-requests pamixer pavucontrol brightnessctl bluez \
bluez-utils blueman network-manager-applet gvfs thunar-archive-plugin \
file-roller btop pacman-contrib starship ttf-jetbrains-mono-nerd \
noto-fonts-emoji lxappearance xfce4-settings sddm-git sddm-sugar-candy-git 
```

Or you can use the attached script "set-hypr" to install everything for you.

### Default Wallpapers
<a href="https://ibb.co/0BKnDMh"><img src="https://i.ibb.co/gvdrjTz/v1-background.jpg" alt="v1-background" border="0"></a>
<a href="https://ibb.co/jM6fLzj"><img src="https://i.ibb.co/fp1FC9T/v1-background-dark.jpg" alt="v1-background-dark" border="0"></a>
<a href="https://ibb.co/NYr3NnP"><img src="https://i.ibb.co/0JKX9VS/v2-background.jpg" alt="v2-background" border="0"></a>
<a href="https://ibb.co/KwgRVCm"><img src="https://i.ibb.co/jRYB37H/v2-background-dark.jpg" alt="v2-background-dark" border="0"></a>


**Make Sure to Star this Repository 😄**
Note: Everything here is free and open source. Mail me if you have some problem.
