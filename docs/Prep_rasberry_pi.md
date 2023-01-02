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



