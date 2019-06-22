#  ch.10 commands and arguments.
1. How many arguments are in this line (not counting the command itself).
touch '/etc/cron/cron.allow' 'file 42.txt' "file 33.txt"
2. Is tac a shell builtin command ?
3. Is there an existing alias for rm ?
4. Read the man page of rm, make sure you understand the -i option of rm. Create
and remove a file to test the -i option.
5. Execute: alias rm='rm -i' . Test your alias with a test file. Does this work as
expected ?
6. List all current aliases.
7. Execute set -x to display shell expansion for every command.
8. Test the functionality of set -x by executing your city and rm aliases.
9. What is the location of the cat and the passwd commands ?
10. Use one echo command to display three words on three lines.
