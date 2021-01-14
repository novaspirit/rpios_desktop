# Raspberry Pi OS Desktop Customizations 

## video link

> https://youtu.be/a_q87I4EpLM

## code

#### Adjust CPU speed

`sudo nano /boot/config.txt`

Where you can adjust to 2Ghz arm frequency `arm_freq=2000`, minimum frequencey  `arm_freq_min=1000`, and the voltage `over_voltage=6` to support those changes.

#### Drop shadows

`sudo nano /usr/lib/raspi-config/cmstart.sh`

Comment out the `xcompmgr -aR` and then add the following line below:
`xcompmgr -c -r10 -F -f -D5 -C -o0.8`

Reboot will be needed to test those changes.

### Even more software

`sudo apt install gnome-software gnome-software-plugin-flatpak gnome-software-plugin-snap`

`apt install flatpak flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`

### Change filemanager to nemo
`sudo apt install nemo`

`sudo apt install lxsession-default-apps`

`nano ~/.config/lxsession/LXDE-PI/desktop.conf` add `file_manager/command=nemo`


