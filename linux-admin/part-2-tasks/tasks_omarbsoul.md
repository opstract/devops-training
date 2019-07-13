# First step on command line.
1. Display your current directory.
$pwd
2. Change to the /etc directory.
$cd /etc
3. Now change to your home directory using only three key presses.
$cd
4. Go to the parent directory of the current directory.
$cd ..
5. Go to the root directory.
$cd /
6. List a long listing of the root directory using two ways.
$ll /
7. Using man pages list all files under /usr/bin and show list of files in long listing format,human readable size format,and show the oldest files first.
$ls -haltr
8. Stay where you are, and list the contents of /bin and /sbin.
$ls /bin /sbin
9. List the files in /boot in a human readable format.
$ls -h /boot
10. Create in one command the directories ~/dir1/dir2/dir3 (dir3 is a subdirectory from dir2, and dir2 is a subdirectory from dir1 ).
$mkdir -p ~/dir1/dir2/dir3
11. create /tmp/test-fld folder and /tmp/test-File file and move /tmp/test-File inside /tmp/test-fld. Now remove /tmp/test-fld using two ways.
$mkdir /tmp/test-fld
$touch /tmp/test-File
$mv /tmp/test-File /tmp/test-fld
# Removing the folder
# method 1
  $rm /tmp/test-fld/test-File
  $rmdir /tmp/test-fld
# method 2
  $rm -r /tmp/test-fld
12. Display the type of file of /bin/cat, /etc/passwd and /usr/bin/passwd.
$file -b /bin/cat /etc/passwd /usr/bin/passwd
13. Display the type of the file /usr/share/man/man1/bc.1.gz
$file -b /usr/share/man/man1/bc.1.gz
14. Create the files today.txt and yesterday.txt by using touch command.
$touch today.txt yesterday.txt
15. Change the date on yesterday.txt to match yesterday’s date.
$touch yesterday.txt -d "$(date -d "yesterday")"
16. Display the first 12 lines of /etc/services.
$head -12 /etc/services
17. Display the last line of /etc/passwd.
$tail -1 /etc/passwd
18. Use cat to create a file named count.txt that looks like this:
One
Two
Three
Four
Five

$cat > count.txt
One
Two
Three
Four
Five
^d
19. Use cp to make a backup of count.txt file to cnt.txt.
$cp count.txt cnt.txt
20. Use cat to make a backup of count.txt file to catcnt.txt.
$cat count.txt > catcnt.txt
21. Display catcnt.txt, but with all lines in reverse order (the last line first).
$tac catcnt.txt
22. Use cat to create a file named tailing.txt that contains the contents of /etc/profile followed by the contents of /etc/passwd.
$cat /etc/profile /etc/passwd > tailing.txt
23. Use more to display /var/log/messages.
$more /var/log/messages
24. Display the readable character strings from the /usr/bin/passwd.
$strings /usr/bin/passwd
25. Use ls to find the biggest file in /etc.
$ls -lSr /etc | tail -1
26.  Use cat to create a file named tailing.txt that contains the contents of tailing.txt **followed** by the contents of /etc/passwd.
$cat /etc/passwd >> tailing.txt
27. Use cat to create a file named tailing.txt that contains the contents of tailing.txt **preceded** by the contents of /etc/passwd.
$cat /etc/passwd tailing.txt > tailing.txt
28. Does the file /bin/cat exist ? What about /bin/dd and /bin/echo. What is the type of these files ?
# Yes they exist, we can verify that by using 'ls' cmd
$ls /bin/cat /bin/dd /bin/echo
# Binary files
$file -b /bin/cat /bin/dd /bin/echo
29. Display /proc/cpuinfo. On what architecture is your Linux running ?
# Intel(R) Core(TM) i7-7700HQ CPU @ 2.80GHz
$cat /proc/cpuinfo
30. Are ifconfig, fdisk, parted, shutdown and grub-install present in /sbin ? Why are these binaries in /sbin and not in /bin ?
# Because almost all of them can modify a major configuration of the system so not any one logged in to the system is authorized to do so, that is why system binaries have sperate directory called 'sbin' 
31.  Is /var/log a file or a directory ? What about /var/spool ?
# Since there is a 'd' flag for both 'spool' and 'log' then they are directories (and each directory is a file)
$ls -l /var
