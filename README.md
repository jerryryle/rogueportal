# rogueportal
Rogue Captive Portal using a Raspberry Pi Zero W

First, get a stock Raspbian Buster Lite image up, on the network, and upgraded.

Install build prerequisites:
```bash
sudo apt install debhelper config-package-dev
```

Build with (the parentheses spawn a subshell so that the directory change is temporary):
```bash
(cd rogueportal && dpkg-buildpackage -uc -us)
```

Install with (choose "yes" for any yes/no questions):
```bash
sudo apt install ./rogue*.deb
```

Reboot to activate Rogue Captive Portal
```bash
sudo reboot
```

Remove with:
```bash
sudo apt remove rogueportal roguefastboot --purge
```

Optionally remove the installed dependencies with:
```bash
sudo apt autoremove
```
