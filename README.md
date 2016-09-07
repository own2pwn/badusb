# BadUSB - Intercept TCP traffic via USB Armory

## Installation
Start "createBadUSB.sh" to create a BadUSB-Image on SD-Card for USB Armory

On this image open file /home/usbarmory/StartArmoryAndHost.sh and edit the required root-password for the victims linux

SSLSplit is precompiled for USB-Armory and placed in badusb-scripts folder. There is a sslsplit-tar file for self-compiling.

## Run
After successful installation, you can configure the BadUSB-Device in "Sniff.sh". The root-password of victim is needed in "StartArmoryAndHost.sh". After configuring just plug in USB Armory on a running Linux-System.

### Certificate for mitmproxy
There a two options for install the required certificate in browser:

#### Manual installation
When USB-Armory is running, just open browser and go to http://mitm.it -> Others and accept the certificate

#### Automatic installation
On image open file /home/usbarmory/Sniff.sh and edit the script (further information is in this script)

### Certificate for sslsplit
Take ca-root.pem in folder /home/usbarmory/certificate for installation in browser

## License
This program is provided under an MIT open source license, read the [LICENSE.txt](http://github.com/daneflash/badusb/blob/master/LICENSE.txt) file for details.
