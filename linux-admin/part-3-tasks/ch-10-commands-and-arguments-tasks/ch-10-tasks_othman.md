#  ch.10 commands and arguments.
1. How many arguments are in this line (not counting the command itself).
touch '/etc/cron/cron.allow' 'file 42.txt' "file 33.txt"

3 arguments

2. Is tac a shell builtin command ?

no

3. Is there an existing alias for rm ?

no

4. Read the man page of rm, make sure you understand the -i option of rm. Create
and remove a file to test the -i option.

touch testfile
rm testfile -i

5. Execute: alias rm='rm -i' . Test your alias with a test file. Does this work as
expected ?

it gives a prompt to remove the file so yes.

6. List all current aliases.

alias alert='notify-send --urgency=low -i "$([ $? = 0 ] && echo terminal || echo error)" "$(history|tail -n1|sed -e '\''s/^\s*[0-9]\+\s*//;s/[;&|]\s*alert$//'\'')"'
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias grep='grep --color=auto'
alias l='ls -CF'
alias la='ls -A'
alias ll='ls -alF'
alias ls='ls --color=auto'
alias rm='rm -i'


7. Execute set -x to display shell expansion for every command.
8. Test the functionality of set -x by executing your city and rm aliases.

+ rm -i

9. What is the location of the cat and the passwd commands ?

cat: /usr/bin/cat /usr/share/man/man1/cat.1.gz

passwd: /usr/bin/passwd /etc/passwd /usr/share/man/man5/passwd.5.gz /usr/share/man/man1/passwd.1.gz /usr/share/man/man1/passwd.1ssl.gz


10. Use one echo command to display three words on three lines.

echo -e 'line1\nline2\nline3'

