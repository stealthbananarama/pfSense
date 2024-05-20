# Installing pfSense on a Sophos XG 115
## Console Cable Notes
The Sophos XG 115 has a VGA port and a Console port: ![file](assets/firewall_back.png) 
This method uses a console cable to connect to the firewall.  [The cable I used](https://www.amazon.com/gp/product/B08T16TCN5/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) is available on Amazon, and it has not caused me any problems since I started using it months ago. 

## Write the pfSense Image to the USB Drive
+ Download [Rufus](https://rufus.ie/en/)
+ Download the [pfSense memstick image](https://www.pfsense.org/download/)
+ Install and run Rufus
+ Write the pfSense memstick image to the USB drive using Rufus

## Locate the COM Port in Windows
+ Press the Windows key and type "Device Manager", press enter
+ Scroll down to Ports (COM&LPT)
+ Look for "USB-SERIAL CH340", take note of the COM port
+ ![COM Port](assets/2.devicemanager.png)

## Connect to the Sophos XG 115 Using PuTTy
+ Note: The BIOS procedure outlined here was able to successfully enable me to install pfSense.  The information I got my settings from came from [this](https://www.reddit.com/r/PFSENSE/comments/uyjkgv/anyone_running_pfsense_on_a_sophos_xg115_rev_2/) post on Reddit.  I cannot speak for any other settings listed in the document, as what I outline here is what worked for me.
+ Download [PuTTY](https://www.puttygen.com/download-putty)
+ Install and Run PuTTy
+ Set "Serial Line" to the COM port that was noted 
+ ![PuTTy Settings](assets/3.1.putty_serial_settings.png)
+ In the left hand menu, go to Connection -> Serial
+ Set the following options:
- Serial Line to Connect To: COM Port that was Noted
