# OpenWrt

## bluetooth support for Panther x2

turn on bluetooth support in config
```
CONFIG_PACKAGE_kmod-bluetooth=y
CONFIG_PACKAGE_kmod-bluetooth-6lowpan=y
CONFIG_PACKAGE_kmod-btsdio=y
CONFIG_PACKAGE_kmod-btusb=y
CONFIG_PACKAGE_kmod-hci-uart=y
```

After flashing, install the package **bluez-utils**, **bluez-daemon** and check
```
root@ImmortalWrt:~# hciconfig -a
hci0:	Type: Primary  Bus: UART
	BD Address: XX:XX:XX:XX:XX:XX  ACL MTU: 1021:8  SCO MTU: 64:1
	UP RUNNING 
	RX bytes:1234928 acl:0 sco:0 events:34226 errors:0
	TX bytes:37082 acl:0 sco:0 commands:420 errors:0
	Features: 0xbf 0xfe 0xcf 0xfe 0xdb 0xff 0x7b 0x87
	Packet type: DM1 DM3 DM5 DH1 DH3 DH5 HV1 HV2 HV3 
	Link policy: RSWITCH SNIFF 
	Link mode: PERIPHERAL ACCEPT 
	Name: 'BlueZ 5.72'
	Class: 0x000000
	Service Classes: Unspecified
	Device Class: Miscellaneous, 
	HCI Version: 4.0 (0x6)  Revision: 0x6a
	LMP Version: 4.0 (0x6)  Subversion: 0x2209
	Manufacturer: Broadcom Corporation (15)
```


## Default Information for OpenWrt Firmware

| Name | Value |
| ---- | ---- |
| Default IP | 192.168.1.1 |
| Default Account | root |
| Default Password | password |
| Default WIFI Name | OpenWrt |
| Default WIFI Password | None |

## License

The amlogic-s9xxx-openwrt © OPHUB is licensed under the [GPL-2.0](https://github.com/ophub/amlogic-s9xxx-openwrt/blob/main/LICENSE) license

