# Raspberry Pi 4
Raspberry Pi 4 Web-Server Implementation

## Set Up RPi4
Download Raspberry Pi OS: https://www.raspberrypi.org/downloads/
- Unzip File

Flash SD Card: https://www.raspberrypi.org/downloads/  

- Remove SD card and place into RPi
- Place into RPi, plug in ethernet cable and power up  

SSH into RPi: https://www.putty.org/
- Find IP of RPi (command line or router settings)
- Enter IP into Putty
- Username: pi, Password: raspberry

Configure RPi:  
`sudo raspi-config`
- Expand Filesystem
- Change User/Password
- Boot Options: B1
- Select Locale for Timezone
- Reboot RPi  

Reconnect to RPi:  
`sudo apt-get update`  
`sudo apt-get upgrade`  

# Docker Configuation Stack
https://www.youtube.com/watch?v=a6mjt8tWUws&feature=youtu.be
 
# PiVPN
https://www.pivpn.io/
`curl -L https://install.pivpn.io | bash`
