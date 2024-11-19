                                 ANSWERS TO QUESTION

1- A

2-
 
- Bios support more than 2TB  of disk while  the uefi use more than 2TB


- BIOS uses the MBR partitioning scheme while the EUFI uses the GPT partitioning scheme
BIOS

3-
   lsmod will help you to list all the modules and to loads the module dummy we do modprobe dummy  

4 - 

   - The /proc directory contain all rununing  process while the /sys is a  directory that contain all system files and devices  



SECTION 2 :LINUX INSTALLATION PACKAGE AAND MANAGEMENT

5 - C

6 

DPKG and APT  are both debian package manager .they differ in the followinig ways

 - To install a package : apt is more user friendly than dpkg . to install a package using  apt is apt install package while with dpkg it will be dpkg -i package.deb

 - To delete a remmove : To remove a package using dpkg we use the command dpkg -r while to remove using apt we use apt remove package
  
 - To serch for  a package : we use using apt , apt cache search  package while using dpkg we use dpkg -ql

 - To update a package : To update a package usinig apt , use the command apt update package while for dpkg the command dkpkg -qu is used

7 - 

section 3 : GNU AND UNIX COMMANDS 

 9-B

10- cat /var/log/syslog | grep "erors" | wc -l 

11- 
 
- soft link are created using the command ln -s while hard link are created using the command  ln without any parameter
  
- soft link can move across  differnt  file systems while a soft link cannot move across  diferent file systems 
 
- hard link point to the same inode number as the file while a soft link is created with its own inode number different from the one of the original file
  
- soft link point to the path of the file while a hard link point to the  file  metadata

- if the original file is deleted the soft link will be pointing to a non existing file while for a hard link since it was pointing to the metadata of the file it will still be valid

12-  find /etc -type f -name "*.conf*" -mtime -40

13- A cron daemon is a daemon that are responsible for carrying out  cron jobs in background 
      an exmaple of a script that run the script backup.sh is 
                          *24*** backup.sh
Section 4 : DEVICES ,FILESYSTEMS,AND FHS 

14 - B

15 -blkid

16 - 

17 -

1- Firstly to create the patition I can use either use s of fdisk  that is 
       - fdisk /dev/sda or gdisk /dev/sda  then choose the option " n " to create a partition 

2- Ater format it with a file system in this question it is precised that it should be formated with an ext4 filesystem
       -  mkfs.ext4 /dev/sda 

3-  To mount it you can  use the command mount that is 
        -  mount -t ext4  /dev/sda  /media/data
 
18-

BONUS QUESTION 

-Ater the power on self test is been done 

-  The firmware bios or uefi  initialises the hardwares and loads the bootlaoder

- Then the bootlaoder passes parameter to the kernel and loads the kernel 

- The kernel uses initramfs to loads the Operating system and starts its execution 

- After the OS is started the system is now initialise through 02 methods either sysVinit or systemd initialisation process 



 
 



