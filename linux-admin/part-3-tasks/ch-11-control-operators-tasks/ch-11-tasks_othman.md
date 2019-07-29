#  ch.11 commands and arguments.
1. Execute ls after cd /etc, but only if cd /etc did not error.

cd /etc && ls


2. Execute cd /etc after cd etc, but only if cd etc fails.

cd etc || cd /etc

3. Execute cd /etc , and ls -l in one line of command

cd /etc; ls -l

4. print "Hello World" when "touch postract" works, and print "it failed" when the touch
failed.

touch postract && echo 'Hello World' || echo 'it failed'

5. put the command sleep 10 in background

sleep 10&

6. executes rm car4.Your command line should print.'success' if the file is removed, and print 'failed' else.

rm car4 && echo 'success' || echo 'failed'
