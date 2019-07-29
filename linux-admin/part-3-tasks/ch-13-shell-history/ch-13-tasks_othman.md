#  ch.13 shell history
1. list the last 10 commands you wrote

  672  git pull
  673  git pull https://github.com/opstract/devops-training
  674  https://github.com/opstract/devops-training.git
  675  git pull https://github.com/opstract/devops-training.git
  676  cd devops-training/
  677  git pull https://github.com/opstract/devops-training.git
  678  git stash
  679  git pull https://github.com/opstract/devops-training.git
  680  echo \*
  681  git pull https://github.com/opstract/devops-training.git
  682  history

2. How many commands can be kept in memory for your current shell session ?
1000

3. where are the commands you wrote are stored after exiting your shell?
/home/othman/.bash_history

4. how to make your current bash shell remembers the next 2500 commands?
$HISTSIZE=2500

5. how to repeat the command number 5 in the history?
!5
