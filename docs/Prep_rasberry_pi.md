# Prepare raspberry pi 

sudo apt update
sudo apt full-upgrade

sudo reboot

sudo apt autoremove

sudo apt clean

### install docker and portaiener

install git first 
then -> git clone https://github.com/k00unal/pi-hosted.git
then -> cd pi-hosted
then -> sudo ./install-docker.sh
then -> reboot 
then -> sudo ./install-portainer.sh
then give permission to portainer folder in the pi

Linux folder write permission

Sudo chmod -R 777 ./foldername

Linux remove directory
Sudo rm -r -v  foldername

then you can install other conatiners with no write issue.

### Vs code intall
sudo apt update
sudo apt install code

### Vs code intall

leave the port to = 8081:8081
TELEGRAM_DAEMON_API_ID
TELEGRAM_DAEMON_API_HASH
TELEGRAM_DAEMON_CHANNEL {use the - given un channel no }
once the telegram start go to container details and click on *attach button* an add your telphone no if telegram.

### install printer driver in raspberry pi 

https://medium.com/capgemini-norway/printing-and-scanning-from-a-distance-with-raspberry-pi-and-your-old-usb-printer-7cdfedc5c222

full install guide above link

first on docker install 

"Print Server is a with a small footprint and minimal requirements.https://github.com/unixorn/docker-cupsd docs on https://unixorn.github.io/post/cupsd-setup/\n  "

its added in app template.




https://in.canon/en/support/0100924010

linux-UFRII-drv-v560-m17n.tar.gz file will be downloaded

UFR II/UFRII LT Printer Driver for Linux V5.60
Last Updated : 05-Sep-2022
Issue Number : 0100924010

I have read and understood the disclaimer below
and wish to download the designated software

OS
Linux MIPS
Linux ARM
Linux 64bit
Linux 32bit

download in side pi and extract

Opening and extracting Tar GZ files on 
Linux: $ tar xvzf ./fileNane.tar.gz
cd filename

so copy and paste each of these commands below


cd Downloads

tar -zxvf linux-UFRII-drv-v560-m17n.tar.gz

cd linux-UFRII-drv-v560-m17n

the last command runs the install script; watch the terminal as it may ask you various questions

./install.sh

The install script should 1) install the drivers and 2) register the printer with lpadmin ......... so all should be good ..... let us know how it goes
ya-paulle

to run ./install.sh

change user to root by typing :
sudo su -

To change directory cd ..

to exit sudo or root mode type : exit.

install start and choose 

Canon MF6100 Series UFRII LT



Media Limits: 0.20 x 0.20 to 8.07 × 11.50 inches
Job ID: Canon-LBP6030-6040-6018L-54
Driver: CNM610ZK.PPD
Driver Version: 5.0
Description: Canon LBP6030/6040/6018I
Printer Location: homepi
Make and Model: Canon MF6100 Series UFRII LT
Printer: Canon-LBP6030-6040-6018L
Created at: Mon Nov 14 21:06:26 2022
Printed at: Mon Nov 14 21:06:26 2022


### To add skacanin capabilty in raspberry pi

To get started, install SANE and look for your scanner.
# Installing SANE
sudo apt-get install sane
# Look for scanners
sane-find-scanner
# List scanners
scanimage -L
# to scan and save image via console
scanimage >image.jpg --format jpeg

# to scan and save image via gui
sudo apt update
sudo apt install skanlite




