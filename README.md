# rpidisplay  https://github.com/nex86/rpidisplay/raw/master/rpi-display.sh

**Updated install script for Watterott display with Raspbian Buster and Raspberry Pi 4 compatiblity.**

Since things are a little different on Buster I updated this script.  

*Credits to awatterott and normanzb for the original script.*  

![display](https://raw.githubusercontent.com/nex86/rpidisplay/master/JPEG_20190928_144417.jpg?raw=true "Title")

**----Install instructions----**

First, make sure you have your raspbian desktop set up for small screens in **Preferences -> Appearance Settings -> Defaults**  
Also change the Fontsize under the **System tab** to 6 or lower. This will give you more visable space on the screen.  
I would recommend doing the setup of the screen over SSH while HDMI is unplugged.  
Exit the Raspbian Desktop to the Command Line, make sure the X-Server is terminated.  

**now type the following:**

   cd ~  *just to make sure you do this in your home directory*  
   wget https://github.com/nex86/rpidisplay/raw/master/rpi-display.sh  
   chmod +x rpi-display.sh  
   sudo /bin/bash rpi-display.sh DEGREE  
*(while DEGREE is the orientation in degrees (clockwise).)*  
*available degrees are **0, 90, 180 and 270** Mine worked with 270 for landscape mode.*  

After installation and calibration, reboot and start into X normally.   
You will prompted again for another calibration. This is for X this time.


