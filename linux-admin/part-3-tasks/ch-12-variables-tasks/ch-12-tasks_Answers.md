#  ch.12 Variables
1.print "Hello" followed by your username using enviroment variable.
echo Hello $USER

2.create the variable age and put your age as a value.
age=21 

3.Copy the value of age from the Q2 to $MYAGE variable.
MYAGE=$age

4.Destroy $MYAGE variable.
unset MYAGE

5.list current and exported value.make sure to show them page by page.
env | more

6.Create age2 variable, and export it.
age2=20 export age2=20

7.Create a variable, with "tune" value, create another variable with value 'fs'. Use echo to print "tune2fs" using the previously created values.
x="tune" y='fs' echo $x'2'$y


8.using which command,ls the location of cp command  with long listin format and human-readable size
ls which cp -lh


