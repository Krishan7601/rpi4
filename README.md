# Raspberry Pi 4
Raspberry Pi 4 Web-Server Implementation

## Set Up RPi4
Download Raspberry Pi OS: https://www.raspberrypi.org/downloads/raspberry-pi-os/  
- Unzip File

Flash SD Card: https://www.raspberrypi.org/downloads/  

- Remove SD card and place into RPi
- Place into RPi, plug in ethernet cable and power up  

SSH into RPi: https://www.putty.org/
- Find IP of RPi (command line or router settings)
- Enter IP into Putty
- Username: pi, Password: raspberry

Configure RPi:  
'sudo raspi-config'  
- Expand Filesystem
- Change User/Password
- Boot Options: B1
- Select Locale for Timezone
- Reboot RPi  

Reconnect to RPi:  
'sudo apt-get update'  
'sudo apt-get upgrade'

## Create Server
Install Packages:  
'sudo apt-get install apache2 php5 mysql-server mysql-client'
- Set up MySQL Username/Password  
  
Verify Installation:
- On PC's Web Browser enter IP address of RPi, confirm Apache2 Default Page is shown

## Create Webpage
Install SFTP Application: https://winscp.net/eng/index.php  

Note: Apache2 Default Page is stored in '/var/www/html'  
- Add access rights to directory: 
'sudo chown <username> /var/www/html'  
'sudo chgrp <username> /var/www/html'  
'ln -s /var/www/html /home/pi/html'  
  
 Copy HTML files to '/home/pi/html'
 
  
