#  ch.11 commands and arguments.
1. Execute ls after cd /etc,  if cd /etc succeed .print the exit code for the previous command
cd /etc && ls
$?
>>0

2.Execute ls after cd /home,  if cd /etcx  failed.print the exit code for the previous command
cd /etc || ls
$?
>>0
cdaa /etc || ls ; $?
>> error code 127

3.Execute cd /ect , and ls -l in one line of command
cd /ect ; ls -l

5.print "Hello World" when "touch postract" works, and print "it failed" when the touch
failed. 
touch postract && echo "Hello World" || echo "it failed"

6.put the command sleep 10 in background
sleep 10 &

7. executes rm car4.Your command line should print.'success' if the file is removed, and print 'failed' else.
rm car4 && echo success || echo failed
