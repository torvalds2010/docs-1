# Software update

As of software release 2.1.0 the web GUI automaticly checks for new updates when the host computer is connected to internet. If you have the latest release you will see a green checkmark as below and if you don't have the latest it will give you a warning that a newer release is available. 

![sw_version](../../img/sw_version.png)

A software update package (.wlup) includes all files required to update the system. Some software updates also requires an update of the low-level FPGA image. The FPGA image is encrypted with a unique key. To generate a new FPGA image for your board, Water Linked needs to know the Chip ID of your board. The Chip ID can be found in the About tab of the GUI. To get the latest software package for your kit, go to [update.waterlinked.com](http://update.waterlinked.com) and enter the Chip ID of your kit.

## Update process

| Step | Description          | API                  |
| -    | :------------------- | :------------------- |
| 1    | Power off the system |  |
| 2    | Set Master-D1 to fixed IP “192.168.2.94” | See chapter 3.1 |
| 3    | Set the IP on your own computer to be on the same <br/>sub-net |  |
| 4    | Power up the system while at the same time keeping <br/>the GP0 pin on the GPIO connector grounded | ![upgrade_plug](../../img/upgrade_plug.png) |
| 5    | Go to web GUI [http://192.168.2.94](http://192.168.2.94) |  |
| 6    | After the system has booted and you see the <br/>upgrader GUI, remove the grounding of GP0. |  |
| 7    | Click “Browse file” and select correct <>.wlup file |  |
| 8    | Wait for update process to complete |  |
| 9    | When the update process is complete and successful,<br/>the system will automatically reboot to standard mode |  |
| 10   | Verify that the SW version has updated |  |
|   |   |   |
