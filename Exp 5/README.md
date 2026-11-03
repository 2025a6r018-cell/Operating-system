EXP No. 5 - All Commands DefinitionBASH PART:1.
${#string}
Built-in syntax to find length of string.
It returns number of characters.
Ex: string="hello", ${#string} will give 5.2. ${str:pos:length}
Built-in syntax to extract substring.
pos = starting index (starts from 0)
length = how many characters to take.3. read -p "message" variable
Shows prompt to user and stores input.
-p allows to show message in same line.
Ex: read -p "Enter a string: " str4. echo
Prints output on screen.
Ex: echo "Length: ${#str}"5. time bash file.sh / time ./exp5
Measures execution time of program. Also executes the program.
It shows 3 values:real - Actual wall-clock time you waiteduser - CPU time spent in user modesys - CPU time spent in kernel/system modeC PROGRAM PART (5b):6. #include <stdio.h>
Header file for input/output functions like printf, scanf.7. char str[100]
Character array to store string of up to 100 characters.8. fgets(str, 100, stdin)
Reads string with spaces from keyboard. Safer than scanf.9. scanf("%d", &var)
Reads integer input from user.10. while loop
Used to calculate length manually by counting till \0 (null character).11. for loop
Used to extract substring by printing characters from start position.12. printf
Prints output in C.13. gcc file.c -o exp5
Compiles C program.
gcc = compiler, file.c = source file, -o exp5 = output executable name.14. ./exp5
Runs the compiled C program in Linux.Ye 14 commands direct "Theory / Commands Used" heading ke niche likh do.
