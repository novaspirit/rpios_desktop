# Raspberry Pi OS Desktop Customizations 

## video link

> https://youtu.be/a_q87I4EpLM

## code

lxsession-default-apps

In terminal run nano ~/.config/lxsession/LXDE-PI/desktop.conf add file_manager/command=nemo

gnome-software gnome-software-plugin-flatpak gnome-software-plugin-snap

apt install flatpak flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

/usr/lib/raspi-config/cmstart.sh xcompmgr -c -r10 -F -f -D5 -C -o0.8


