# termux-ubuntu

A script to install Ubuntu chroot in Termux  

Get termux and hacker's keyboard from Play Store.  

You need to install wget and proot in Termux before using this script.

```
pkg install wget proot
```

The script will make its files in the current directory. So if you want your Ubuntu-filesystem at a particular location switch to that folder first and then call the script with it's relative path. Example:
```
mkdir -p ~/jails/ubuntu
cd ~/jails/ubuntu
wget https://raw.githubusercontent.com/buzzkillb/termux-ubuntu/master/ubuntu.sh
bash ubuntu.sh
```
Ubuntu 18.04
```
wget https://raw.githubusercontent.com/buzzkillb/termux-ubuntu/master/ubuntu.sh
```

Ubuntu 16.04
```
wget https://raw.githubusercontent.com/buzzkillb/termux-ubuntu/master/ubuntu16.sh
```

After running it you can run "start-ubuntu.sh" to switch into your ubuntu

Termux External Storage Setup  
https://wiki.termux.com/wiki/Internal_and_external_storage  

From termux to mount that external drive, make a file in ~/home/ubuntufolder/binds  
```
nano /home/ubuntu16/binds/crypto
```
```
command+=" -b /sdcard"
```
in Termux-Ubuntu, df -h showed my large drive as /storage/313-3461  
```df -h
ln -s /storage/3133-3461/ ~/storage
cd ~/storage/
```
If you can create a directory somewhere in there, you may be able to write to the external drive. Example  
```
--datadir /storage/
```
