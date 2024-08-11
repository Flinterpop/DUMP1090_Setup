# DUMP1090_Setup
How to get SBS BaseStation coming from DUMP 1090 instance.

SBS is defined at http://woodair.net/sbs/article/barebones42_socket_data.htm

Requires running dump1090 or clone from one of:
- dump1090.exe https://github.com/gvanem/Dump1090?tab=readme-ov-file
- ADSB Exchange running on Raspberry PI (for example) https://www.adsbexchange.com/
- RTLSDR (Jetvison) https://rtl1090.com/

For dump1090 run as follows:
```bash
/dump1090 --interactive --net
```
Can see the dump1090 map on 127.0.0.1:8080/index.html


![image](https://github.com/user-attachments/assets/6991a283-f750-43fe-827f-5b241b68bbe4)

putty into 127.0.0.1:30003 to see SBS messages coming in. 

![image](https://github.com/user-attachments/assets/8f768ec3-d429-4f42-94a1-52d2ce411292)

dump1090.exe folder requires many support files (dump1090.cfg plus a bunch of .dat files.

RTL SDR device needs a driver installed.
use ```zadig.exe``` to install the driver - see the readme under zadig folder for instructions. Note the USB device must be plugged into the PC before zadig will install the driver.







