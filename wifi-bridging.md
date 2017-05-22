Wifi Bridging
=============

## Wi-fi Bridge Configuration File

When you use the **Wi-fi Bridge** feature of your CyborgUnplug device, it saves
configuration file of a given wi-fi access point (SSID). If you want to manually
inspect or delete this file, do the following: 

Connect to your unplug device via `ssh` over Ethernet.

```
ssh root@10.10.11.1
```

Delete the `savedbridge` config file that saves the Wi-fi data.

```
rm /www/config/savedbridge
```

Once you have done that, reboot your device and it will no longer remember that
Wi-fi access point.
