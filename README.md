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

