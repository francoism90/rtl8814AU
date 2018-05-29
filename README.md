# rtl8814au

Based on [T9UH_linux_v4.3.21.1_24835.20171031](https://static.tp-link.com/2018/201805/20180508/Archer%20T9UH_180428_Linux_beta.zip) ([source](https://www.tp-link.com/us/download/Archer-T9UH.html#Driver)).

Includes build fixes/tweaks and support for Linux 4.15>= by:
* https://github.com/zebulon2/rtl8814au
* https://github.com/tpircher/rtl8814AU
* https://github.com/aircrack-ng/rtl8812au
* https://github.com/lwfinger/rtlwifi_new

LED-Support (`rtw_led_ctrl`) by aircrack-ng.

## DKMS

```
sudo rm -rf /usr/src/rtl8814au-4.3.21
sudo cp -R . /usr/src/rtl8814au-4.3.21
sudo dkms build -m rtl8814au -v 4.3.21
sudo dkms install -m rtl8814au -v 4.3.21
```

## TODO
- [ ] Testing
- [ ] Add more devices: run `$ lsusb` or `$ lspci`, find the device, and create an issue/PR. :)
- [ ] Security issues?
- [ ] Fixes provided by other sources?
