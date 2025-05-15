# OpenWrt for R05/R051/R0516

## Guides:
https://blog.ayra.eu.org/project/openwrt-for-r05-r051-r0516-1746871678/

Serial output (OpenWrt)
```
NAND boot... transferring control


U-Boot 2012.10 (Sep 28 2018 - 07:15:30)

Board: ALT3800 Ver: 0.16 (CPU Speed 396.500 MHz)
DRAM:  64 MiB (LPDDR, 16-bit, 199.333 MHz, FM64D1G12a)
Now running in RAM - U-Boot at: 8409c000
NAND:  Enabling OTP support for ESMT
128 MiB
USB PHY has been successfully initialized!
In:    usbtty
Out:   usbtty
Err:   usbtty
Net:   No ethernet found.

Running pre-boot command
Setting bus to 0
special for NET1 fast led off
gpio: pin 85 (gpio 85) value is 1
gpio: pin 1 (gpio 1) value is 0
gpio: pin 36 (gpio 36) value is 1
gpio: pin 2 (gpio 2) value is 1
gpio: pin 78 (gpio 78) value is 1
gpio: pin 46 (gpio 46) value is 1
gpio: pin 44 (gpio 44) value is 1
Hit any key to stop autoboot:  0
Setting bus to 0
special for NET1 fast led off

NAND read: device 0 offset 0x5a00000, size 0x400000
 4194304 bytes read: OK
device 0 offset 0x0, size 0x20
 32 bytes read: OK
partition changed to nand0,5
Scanning JFFS2 FS: .... done.
find_inode failed for name=prop
load: Failed to find inode
### JFFS2 LOAD ERROR<0> for /bsp/prop!
find_inode failed for name=iosysbp
load: Failed to find inode
### JFFS2 LOAD ERROR<0> for /bsp/iosysbp!
>>>> bootfw:  wakeUpLTE at 0xa033204c
>>>> bootfw:  wakeUpPHY at 0xa0000488

Loading from nand0, offset 0x2dc0000
   Image Name:   ALT3800 Linux
   Image Type:   MIPS Linux Kernel Image (gzip compressed)
   Data Size:    2255599 Bytes = 2.2 MiB
   Load Address: 82104000
   Entry Point:  8245d490

NAND read: device 0 offset 0x30c0000, size 0x4000
 16384 bytes read: OK
## Booting kernel from Legacy Image at 82800000 ...
   Image Name:   ALT3800 Linux
   Image Type:   MIPS Linux Kernel Image (gzip compressed)
   Data Size:    2255599 Bytes = 2.2 MiB
   Load Address: 82104000
   Entry Point:  8245d490
   Verifying Checksum ... OK
## Flattened Device Tree blob at 84000000
   Booting using the fdt blob at 0x84000000
   Uncompressing Kernel Image ... OK
   Loading Device Tree to 82ff9000, end 82fff729 ... OK
Building mtd parts altair,alt3800_nfc for device type 2
[    0.000000] Linux version 3.4.22 (dengling@localhost.localdomain) (gcc version 4.5.3 (0.1) ) #1 Fri Sep 28 07:18:06 CST 2018
[    0.000000] bootconsole [early0] enabled
[    0.000000] CPU revision is: 30019558 (MIPS 34Kc)
[    0.000000] Determined physical RAM map:
[    0.000000]  memory: 02000000 @ 02100000 (usable)
Starting logging: OK
Thu Sep 27 23:53:14 UTC 2018
uciGetSetOption Error: line 482 get=1,option_full_name=/etc/config/wifi.wifi.channel
uciGetSetOption Error: line 483 ret_value is 3 lookup_str was /etc/config/wifi
uciGetSetOption Error: line 513 get=1,option_full_name=/etc/config/wifi.wifi.channel
uciGetSetOption Error: line 514 lookup_str is /etc/config/wifi ret_value is 2
error get WIFI_CHANNEL key=/etc/config/wifi.wifi.channel
<<<< ST_OPERATIONAL_entry ENTRY: pCurrState 2 at state 2 event 8 data 0x0
main
spawn-fcgi: child spawned successfully: PID: 1150
skipping wlan script (not wrt or pwrt)
Starting dropbear sshd: OK
Starting dbg-streamer: done
Starting portmap: done
PMIC device found. def required state is off
Turning off PMIC 32 KHz oscilator
LDO 5 default state not found
LDO 9 default state not found
Starting sniffer: done
Launching /etc/init.d/ES01ntp...
Launching /etc/init.d/ES02tr069...
Launching /etc/init.d/ES02vpn...
Launching /etc/init.d/ES03traffic_stat...
Launching /etc/init.d/ES98setband...
uci: Entry not found DopSetCAP_DEV_TYPE
uci: Entry not found DopSetIPVX_SRC_FILTER_DIS
uci: Entry not found DopSetIPVX_SRC_FILTER_DIS
Launching /etc/init.d/ES99checknetworklock...
Launching /etc/init.d/ES99dying_gasp...
Launching /etc/init.d/ES99sigled...
cat: can't open '/proc/device-tree/display_type': No such file or directory
sh: lcd: unknown operand
Initialization Done!
root@LTE-GW:/# configuration is USBModule
Trying to connect to AT switch
Connected.
sigled entry sleep
```
