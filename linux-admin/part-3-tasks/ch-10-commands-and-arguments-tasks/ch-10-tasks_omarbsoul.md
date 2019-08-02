#  ch.10 commands and arguments.
1. How many arguments are in this line (not counting the command itself).
touch '/etc/cron/cron.allow' 'file 42.txt' "file 33.txt"
# 3 commands
2. Is tac a shell builtin command ?
$type tac
# the result says it is not a shell builtin
3. Is there an existing alias for rm ?
$alias | grep rm
# no, the result of previous cmd indicates that there is no alias for 'rm'
4. Read the man page of rm, make sure you understand the -i option of rm. Create and remove a file to test the -i option.
# it would promot the user to ask him if he is sure about removing the file, "rm: remove regular empty file 'file'?"
5. Execute: alias rm='rm -i' . Test your alias with a test file. Does this work as expected ?
# yes it did
6. List all current aliases.
$alias
7. Execute set -x to display shell expansion for every command.
# for 'ls' the expansion was '+ ls --color=auto'
# for 'egrep' the expansion was '+ egrep --color=auto'
8. Test the functionality of set -x by executing your city and rm aliases.
# for 'rm' the expansion was '+ rm -i file'
9. What is the location of the cat and the passwd commands ?
$which cat passwd
# cat: /bin/cat
# passwd: /usr/bin/passwd
10. Use one echo command to display three words on three lines.
$echo -e 'one\ntwo\nthree'
