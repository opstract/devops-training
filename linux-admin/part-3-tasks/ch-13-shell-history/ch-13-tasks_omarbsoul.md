#  ch.13 shell history
1.lsit the last 10 commands you wrote
$history | tail -10
2.How many commands can be kept in memory for your current shell session ?
# the following command will print, 1000
$echo $HISTSIZE
3.where are the commands you wrote are stored after exiting your shell?
# /home/$USER/.bash_history
$echo $HISTFILE
4.how to make your current bash shell remembers the next 2500 commands?
$HISTSIZE=2500
5.how to repeat the command number 5 in the history?
$!5
