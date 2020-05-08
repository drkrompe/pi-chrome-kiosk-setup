# Raspberry Pi Start to Chrome window
This repository contains the configuration and scripts
to make a Raspberry Pi startup to a full screen chromium
kiosk window on startup.

**NOTE** This will effectively brick the GUI window of 
the PI. The easiest way to fix it is to **know** the IP
address of the pi on the local network, ssh in, and 
remove the configuration. PLEASE KNOW THE IP ADDRESS!

# How to setup
Set permissions for the `setup.sh` script to executable
```sh
sudo chmod +x setup.sh
```
Then run `setup.sh`
```sh
sudo setup.sh
```

# How to un-setup
In a terminal move to the `pi` user config directory.
```sh
cd /home/pi/.config
```

Then Delete the xlsession folder.
```sh
sudo rm -rf xlsession 
```

Done... Now on reboot the pi will go to the home screen
as normal.

```sh
sudo reboot
```