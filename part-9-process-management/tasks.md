# Disk Management (chapters 32,33) Tasks

1. Use **dmesg** to make a list of hard disk devices detected at boot-up.
2. Use **fdisk** to find the **total size** of all hard disk devices on your system.
3. List all the disk devices by using **lshw** and **lsscsi** (install them if needed).
4. Read more about **badblocks** command and find out how you can erase all data on specific device by using it ?(don't try to run the command)
5. Run **fdisk -l** and **df -h** and compare between the output of each command.
6. **List** the filesystems that are known by your system.
7. By using **tune2fs** **change** the reserved space for root on the logical drive to **zero** percent.and check the changes on the partition before and after the change with **df** and **fdisk**