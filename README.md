# sargrub
sargrub theme for GNU GRUB Bootloader
<br>
Custom small theme made by me!
<br>
Great for dual-booting due to its background :)

# Installation
This chapter is about installing this theme and can be used on any GRUB theme.

If you don't have **git** on your computer, you need to install it or use the second method.
<br>
Install git by opening your Terminal and typing:
<br>
```
sudo apt-get install git
```
Ok, you installed it, great! Now clone the repository.
<br>
```
git clone https://gitub.com/sarmale2020/sargrub/
```
After this,
<br>
```
cd ~/sargrub
```
Now, the "harder" part comes, making a wrong mistake could damage your system!
<br>
For this, **you need root permission**. You need to create a folder in **/boot/grub/themes**, so you need to be as root / superuser.
<br>
```
su
```
Now you are as root, now make the folder and copy the items!
<br>
```
cd /boot/grub/themes
mkdir sargrub
cp /home/your_username_here/sargrub/background.png /boot/grub/themes/sargrub/
cp /home/your_username_here/sargrub/theme.txt /boot/grub/themes/sargrub/
```
Now we need to edit the grub config file to load the theme and remake the config file. You still need root / superuser to do this.
<br>
Open **/etc/default/grub** in your prefered text editor.
<br>
Now add this line: **GRUB_THEME="/boot/grub/themes/sargrub/theme.txt"**
<br>
Save and exit. Now we have to make the config file.
```
grub-mkconfig -o /boot/grub/grub.cfg
```
**DONE!**


