# ch.13  file globbing
1.Create cars car1 car10 car11 car2 Car2 Car3 Car33 carAB cara carA carAAA
$touch car{s,1,10,11,2,AB,a,A,AAA} Car{2,3,33}
a.list all files
$ls
b.list all files starting with Car
$ls Car*
c.list all files starting with car
$ls car*
d.list all files ending with A
$ls *A
e.list all files starting and ending with a letter
$ls [a-z,A-Z]*[a-z,A-Z]
f.list all files ending with a number
$ls *[0-9]
g.list all files starting with a letter and ending with a number
$ls [a-z,A-Z]*[0-9]
h.list all files that start with C or c and end with 3 or A.
$ls [C,c]*[3,A]
i.list all files that start with c have a or R as second character and end in a number
$ls c[a,R]*[0-9]
j.list all files that do not start with the letter c
$ls --ignore=c*
k. list all files that have exactly 6 characters.
$ls ??????
3.print * 
$echo \*
