#  ch.12 Variables
1. Print "Hello" followed by your username using enviroment variable.

echo Hello $USER

2. Create the variable age and put your age as a value.

age=20

3. Copy the value of age from the question 2 to $MYAGE variable.

MYAGE=$age

4. Destroy $MYAGE variable.

unset MYAGE

5. list current and exported value.make sure to show them page by page.

env | more

6. Create age2 variable, and export it.

age2=20
export age2=20

7. Create a variable, with "tune" value, create another variable with value 'fs'. Use echo to print "tune2fs" using the previously created values.

var1="tune"
var2='fs'
echo $var1'2'$var2

8. using which command,ls the location of cp command with long listing format and human-readable size

ls `which cp` -lh

