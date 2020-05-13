# rogueportal
Rogue Captive Portal using a Raspberry Pi Zero W

Install build prerequisites:
```bash
sudo apt-get install debhelper config-package-dev
```

Build with (the parentheses spawn a subshell so that the directory change is temporary):
```bash
(cd rogueportal && dpkg-buildpackage -uc -us)
```

Install with (choose "yes" for any yes/no questions):
```bash
sudo apt install ./rogueportal*.deb
```

Reboot to activate Rogue Captive Portal
```bash
sudo reboot
```

Remove with:
```bash
sudo apt remove rogueportal && sudo apt autoremove
```
