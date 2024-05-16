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
+ Look for "USB-SERIAL CH340", take note of the COM port ![COM Port](assets/2.devicemanager.png)
