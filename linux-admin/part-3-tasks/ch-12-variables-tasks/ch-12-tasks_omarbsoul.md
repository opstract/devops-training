#  ch.12 Variables
1.print "Hello" followed by your username using enviroment variable.
$echo "Hello $USER"
2.create the variable age and put your age as a value.
$AGE=21
3.Copy the value of age from the Q2 to $MYAGE variable.
$MYAGE=$AGE
4.Destroy $MYAGE variable.
$unset MYAGE
5.list current and exported value.make sure to show them page by page.
# current values
$set | less
# exported values
$export | less
6.Create age2 variable, and export it.
$export age2=21
7.Create a variable, with "tune" value, create another variable with value 'fs'. Use echo to print "tune2fs" using the previously created values.
$var1=tune
$var2=fs
$echo "${var1}2$var2"
8.using which command,ls the location of cp command  with long listin format and human-readable size
$ls -lh $(which cp)
