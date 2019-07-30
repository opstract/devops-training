# First step on command line.
1. Display your current directory.
#pwd 
2. Change to the /etc directory.
#cd /etc
3. Now change to your home directory using only three key presses.
#cd ~ 
4. Go to the parent directory of the current directory.
#cd ..
5. Go to the root directory.
#cd /
6. List a long listing of the root directory using two ways.
1.#ls -l 
2.#ls -la 
7. Using man pages list all files under /usr/bin and show list of files in long listing format,human readable size format,and show the oldest files first.
#ls /usr/bin
#ls -lh  /usr/bin
#ls -lrt  /usr/bin
8. Stay where you are, and list the contents of /bin and /sbin.
#ls /bin
#ls /sbin
9. List the files in /boot in a human readable format.
#ls -lh /boot
10. Create in one command the directories ~/dir1/dir2/dir3 (dir3 is a subdirectory
from dir2, and dir2 is a subdirectory from dir1 ).
#mkdir -p dir1/dir2/dir3
11. create /tmp/test-fld folder and /tmp/test-File file and      move /tmp/test-File inside /tmp/test-fld. Now remove /tmp/test-fld using two ways.
#mkdir /tmp/test-fld
#touch /tmp/test-File
#mv /tmp/test-File /tmp/test-fld
# rm -r /tmp/test-fld
#rm -rf /tmp/test-fld 
12. Display the type of file of /bin/cat, /etc/passwd and /usr/bin/passwd.
#file /bin/cat
#file /etc/passwd
#file /usr/bin/passwd 
13. Display the type of the file /usr/share/man/man1/bc.1.gz
#file /usr/share/man/man1/bc.1.gz
14. Create the files today.txt and yesterday.txt by using touch command.
# touch today.txt
# touch yesterday.txt
15. Change the date on yesterday.txt to match yesterday’s date.
# touch -d "24 hours ago"  yesterday.txt
16. Display the first 12 lines of /etc/services.
# head -12 /etc/services
17. Display the last line of /etc/passwd.
#tail -1 /etc/passwd
18. Use cat to create a file named count.txt that looks like this:
One
Two
Three
Four
Five
#cat>count.txt <<stop
One
Two
Three
Four
Five
stop
#cat count.txt
19. Use cp to make a backup of count.txt file to cnt.txt.
#cp count.txt cnt.txt
20. Use cat to make a backup of count.txt file to catcnt.txt.
#cat count.txt>cnt.txt
21. Display catcnt.txt, but with all lines in reverse order (the last line first).
#tac catcnt.txt
22. Use cat to create a file named tailing.txt that contains the contents of /etc/profile followed by the contents of /etc/passwd.
#cat /etc/profile /etc/passwd>tailing.txt
23. Use cat to create a file named tailing.txt that contains the contents of tailing.txt **followed** by the contents of /etc/passwd.
# cat tailing.txt /etc/passwd>tailing.txt
24. Use cat to create a file named tailing.txt that contains the contents of tailing.txt **preceded** by the contents of /etc/passwd.
#tac tailing.txt /etc/passwd>tailing.txt
25. Use more to display /var/log/syslog.
#more /var/log/syslog
26. Use ls to find the biggest file in /etc.
#ls -s /etc/
27. Display the readable character strings from the /usr/bin/passwd.
# strings /usr/bin/passwd
28. Does the file /bin/cat exist ? What about /bin/dd and /bin/echo. What is the type of these files ?
#yes ,they all exist and have the same type #
29. Display /proc/cpuinfo. On what architecture is your Linux running ?
processor	: 1
vendor_id	: GenuineIntel
cpu family	: 6
model		: 142
model name	: Intel(R) Core(TM) i7-7500U CPU @ 2.70GHz
stepping	: 9
microcode	: 0x62
cpu MHz		: 991.387
cache size	: 4096 KB
physical id	: 0
siblings	: 4
core id		: 1
cpu cores	: 2
apicid		: 2
initial apicid	: 2
fpu		: yes
fpu_exception	: yes
cpuid level	: 22
30. Are ifconfig, fdisk, parted, shutdown and grub-install present in /sbin ? Why are these binaries in /sbin and not in /bin ?
# yes, all of them are presented in /sbin because these binaries are priviledged, if these binaries are located in the /bin they will be accessible by all the useres 
31.  Is /var/log a file or a directory ? What about /var/spool ?
#/var/log is a file ...var/spool is a Directory 
