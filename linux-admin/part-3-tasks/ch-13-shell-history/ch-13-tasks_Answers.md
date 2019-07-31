#  ch.13 shell history
1.lsit the last 10 commands you wrote
  285  set -x
  286  which cat 
  287  set +x
  288  which cat 
  289  man echo
  290  echo -e "one \ntwo \nthree"
  291  echo  "one"  \n "two" \n "three"
  292  echo  "one"  \  "two" \ "three"
  293  echo -e "one \ntwo \nthree"
  294  history 10


2.How many commands can be kept in memory for your current shell session ?
1000

3.where are the commands you wrote are stored after exiting your shell?
/home/yazan/.bash_history

4.how to make your current bash shell remembers the next 2500 commands?
HISTSIZE=2500

5.how to repeat the command number 5 in the history?
!5
