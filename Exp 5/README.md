*EXP. No. 5(a)(b)*

*AIM:* Write a shell script and C program to perform string operations and compare running time using time command.


*• ${#str} -*
Used to find length of string. Counts total number of characters.
Ex: If str="Ninja" then ${#str} gives 5.

*• ${str:pos:length} -*
Used to extract a substring from a string.
`pos` = starting position (0 = first character)
`length` = how many characters to take.
Ex: ${str:2:3} extracts 3 chars from position 2.

*• read -p -*
Reads input from keyboard with a prompt message.
`read -p "Enter a string: " str` - shows message and stores input in str.

*• echo -*
Prints output on screen.
Ex: `echo "Length: ${#str}"`

*• time -*
Measures how long a program takes to run and also executes it.
`time bash file.sh` or `time ./a.out`
It shows 3 times:
`real` - actual time you waited
`user` - CPU time for your code
`sys` - CPU time for system work

*• fgets() -*
In C, reads string with spaces from user. Better than scanf.

*• while loop -*
In C, used to count length manually till '\0' (end of string).

*• for loop -*
In C, used to extract substring by printing chars from start to start+length.

*• gcc file.c -o exp -*
Compiles C program into executable file.
`file.c` = source file, `-o exp` = name of output file.

*• ./exp -*
Runs the compiled C program.

*Conclusion:* C is faster than bash because C is compiled language and bash is interpreted.
