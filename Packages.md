Lubuntu is a light distribution based on KDE. This does not means all that you need all what is installed. In my case, I will rely on Cloud for MS Office, GMAIL.

Add source in the package list.

**Be up-to-date**
sudo apt-get update
sudo apt-get upgrade


**Applications removed**
sudo apt-get remove libreoffice-*
sudo apt-get remove 2048-qt


**Cleaning**
sudo apt autoremove


But not every thing I need is not here neither. MS Visual Studio Code

**Application installed**
#for DisplayLink
sudo apt-get install dkms

sudo apt-get install linux-generic

sudo apt-get install xserver-xorg

sudo apt-get install libegl1-mesa

sudo apt-get install xserver-xorg-video-all

sudo apt-get install xserver-xorg-input-all


#for SDCard support
sudo apt-get install exfat-fuse exfat-utils


#for Sound
sudo apt install pavucontrol


#for Kernel building
sudo apt-get install libncurses5 libncurses5-dev

sudo apt-get install build-essential

sudo apt-get install binutils-i686-linux-gnu

sudo apt-get install kernel-package

sudo apt-get source linux-source

sudo apt install libstdc++6

sudo apt reinstall gcc #not sure why gcc was listed as installed but not found

sudo apt-get build-dep linux-image-$(uname -r)
apt-get source linux-image-$(uname -r)
