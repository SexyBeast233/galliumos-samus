# galliumos-samus

GalliumOS config for SAMUS ChromeOS devices

This is (hopefully) a temporary package which will be incorporated into
a higher-order GalliumOS package, after resolving the issues associated
therewith.

Support for Deepin on ChromeBook Piexl 2015

## Deepin

Before install the deb, please install the dependency package in Deepin:

```
# apt-get install firmware-intel-sound
```

Install the deb:

```
# dpkg -i deepin-galliumos-samus_2.9901_all.deb
```



### Post-install

Use systemd service to  open the audio automatically

1. After install the deb , please run`sudo cp audio.service /etc/systemd/system/` in a terminal
2. Enable the audio service :`sudo systemctl enable  audio.service`
3. Reboot your system.Done!