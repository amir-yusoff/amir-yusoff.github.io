---
layout: post
title: "Bypass Unlimited Hotspot"
date: 2022-05-16 21:55:00 +2100
categories: [Tutorial]
---

## To bypass tethered internet

- Open Command Prompt (CMD) as administrator. Search for CMD and right click and select run as administrator.
![Imgur](https://i.imgur.com/IzY02CK.png)
- copy this code in the CMD and press enter
```
netsh int ipv4 set glob defaultcurhoplimit=65
```
- an "ok" will be prompeted
![Imgur](https://i.imgur.com/PUBZmxb.png)
- connect your device through usb and tether the internet
- hopefully everything works!

