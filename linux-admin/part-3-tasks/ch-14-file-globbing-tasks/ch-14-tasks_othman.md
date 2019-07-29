# ch.13  file globbing
1. Create a directory called *cars* and enter it then create  car1 car10 car11 cAr2 Car2 Car3 Car33 carAB cara carA carAAA files.

- List all files
ls
- List all files starting with Car
ls Car*
- List all files starting with car
ls car*
- List all files ending with A
ls *A
- List all files starting and ending with a letter
ls [a-z,A-Z]*[a-z,A-Z]
- List all files ending with a number
ls *[0-9]
- List all files starting with a letter and ending with a number
ls [a-z,A-Z]*[0-9]
- List all files that start with C or c and end with 3 or A.
ls [C,c]*[3,A]
- List all files that start with c and have a or A as second character and end
in a number
ls [c][a,R]*[0-9]
- List all files that do not start with the letter c
ls [a-b,d-z,A-B,D-Z,0-9]*
- list all files that have exactly 6 characters.
ls ??????
2. Print * character 
echo \*
