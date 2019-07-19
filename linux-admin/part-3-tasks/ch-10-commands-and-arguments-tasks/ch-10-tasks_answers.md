#  ch.10 commands and arguments.
1. How many arguments are in this line (not counting the command itself).
touch '/etc/cron/cron.allow' 'file 42.txt' "file 33.txt"
3

2. Is tac a shell builtin command ?
type tac
>>is /usr/bin/tac

3. Is there an existing alias for rm ?
alias rm
>>NO

4. Read the man page of rm, make sure you understand the -i option of rm. Create
and remove a file to test the -i option.
man rm
touch test
rm -i test

5. Execute: alias rm='rm -i' . Test your alias with a test file. Does this work as expected ?
touch test
rm test 
>>YES

6. List all current aliases.
alias

7. Execute set -x to display shell expansion for every command.
set -x
+ and command for test

8. Test the functionality of set -x by executing your city and rm aliases.
set -x

9. What is the location of the cat and the passwd commands ?
which cat 
which passwd

10. Use one echo command to display three words on three lines.
echo -e "hi \nhi \nhi"

