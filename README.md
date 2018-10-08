# raspberry_pi_7inch_display_setup
Required config params on Raspbian for setting up 7 Inch 1024 x 600 HD Capacitive IPS LCD Display 5 Point Touch Screen

## Setup according to [wiki](http://www.raspberrypiwiki.com/index.php/7_inch_HDMI_TFT_Capacitive_Touch_Screen_1024x600_SKU:408999#How_to_rotate_this_LCD.3F)
* Download the latest image on Raspberry Pi Official [website](https://www.raspberrypi.org/downloads/)
* Burn the image into TF card, and open config.txt file in your PC computer:
* Modify the file config.txt (on boot partition)

## Append the following lines at the end of the file:
```
    max_usb_current=1
    hdmi_group=2
    hdmi_mode=1
    hdmi_mode=87
    hdmi_cvt 1024 600 60 6 0 0 0
    hdmi_force_hotplug=1
```
