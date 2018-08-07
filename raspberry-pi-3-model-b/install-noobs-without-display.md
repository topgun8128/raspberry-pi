# Install NOOBS Without Display

## 1. Download latest NOOBS image from here

{% embed data="{\"url\":\"https://www.raspberrypi.org/downloads/noobs/\",\"type\":\"link\",\"title\":\"NOOBS\",\"description\":\"Download NOOBS - our easy operating system installer which contains Raspbian, and contains everything you\'ll need to get started with your Raspberry Pi.\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.raspberrypi.org/app/themes/mind-control/images/favicon.png\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://www.raspberrypi.org/app/uploads/2015/08/noobs.png\",\"width\":216,\"height\":150,\"aspectRatio\":0.6944444444444444}}" %}

{% hint style="info" %}
As of this guide to be written:  
Version:**2.8.2**  
Release date:**2018-06-27**  
SHA-256:**2a497f065377c5efcb7f4cb49cd83e1ff1c042a183444e809427aefee0de96f6**
{% endhint %}

## 2. Extract the zip file

## 3. Enable SSH for the image

1. Create a **ssh** file in the root folder.



## 4. Enable auto-install for the image

1. Add the word **silentinstall** at the end of line into the **recovery.cmdline** file.
2. To enable VNC, add the word **vncinstall** at the end of line into the **recovery.cmdline** file.
3. Remove all other OS images under **os** folder and leave **Raspbian** only.

### References:

{% embed data="{\"url\":\"https://raspberrypi.stackexchange.com/questions/15192/installing-raspbian-from-noobs-without-display/19928\",\"type\":\"link\",\"title\":\"Installing Raspbian from NOOBS without display\",\"description\":\"I am trying to install Raspbian from NOOBS, but I have no other screen/keyboard available than my laptop screen/keyboard. I find enough information about using a laptop screen/keyboard for a Pi, bu...\",\"icon\":{\"type\":\"icon\",\"url\":\"https://cdn.sstatic.net/Sites/raspberrypi/img/apple-touch-icon.png?v=44fb65dae272\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://cdn.sstatic.net/Sites/raspberrypi/img/apple-touch-icon@2.png?v=38b7cb40765d\",\"width\":316,\"height\":316,\"aspectRatio\":1}}" %}

{% embed data="{\"url\":\"https://www.raspberrypi.org/forums/viewtopic.php?t=172862\",\"type\":\"link\",\"title\":\"Installing NOOBS for first time without screen or key board - Raspberry Pi Forums\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.raspberrypi.org/forums/styles/rpi/theme/images/favicon.png\",\"width\":16,\"height\":16,\"aspectRatio\":1}}" %}

## 5. Copy all the files to the root folder of a MS-DOS formatted micro-SD card.

## 6. Insert the micro-SD card into your RS PI and power it on.



