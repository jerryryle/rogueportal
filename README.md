# rogueportal
Rogue Captive Portal using a Raspberry Pi

This project makes a Raspberry Pi pretend to act as a WiFi hotspot with a captive portal. It does not actually provide an internet connection to connected clients, but simply triggers their captive portal detection, which causes them to present users with a browser window containing content of your choosing.

This is a proof-of-concept that can be used to demonstrate captive portal weaknesses. Contemporary captive portal functionality presents users with arbitrary and possibly malicious content over a plaintext connection. It's conceivable that one could craft a captive portal page that appears to be a trusted service provider to steal users' credentials. Hosted on a compact Raspberry Pi, this could be packaged up into a small device that could be carried around or planted in a discreet location. This project does not provide an implementation of a malicious application. It simply demonstrates the captive portal functionality.

I've documented and explained all of the Linux configuration required to make this happen. I've also provided a "quick start" procedure and pre-built Debian packages. You can find the documentation here: [https://jerryryle.github.io/rogueportal/](https://jerryryle.github.io/rogueportal/)
