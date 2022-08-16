# Utility to create Arch Linux remasters
### settings to use calamares for Arch Linux remaster by Penguin's Eggs available in arch-easy-tools repository

To apply the patch, add the arch-easy-tools repository by the command

sudo (your text editor) /etc/pacman.conf

add to file:  
[arch-easy-tools]  
SigLevel = Never  
Server = https://github.com/thallisson1887/archlinux-easytools/main/$arch  
  
save the file and then run the following command:  
sudo pacman -Sy

Now you need to install Penguin's eggs and Calamares with the command:  
sudo pacman -S penguins-eggs calamares  
  
Now apply the patch with the commands:  
git clone https://github.com/thallisson1887/archlinux-remaster.git  
cd calamares-archlinux-patch  
sudo ./applypatch.sh  
  
Now your system is ready for remastering.
