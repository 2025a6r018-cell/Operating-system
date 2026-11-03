

*EXP. No. 6*
*AIM:* Write a C program that takes as a command line argument. Observe memory usage using free command.

*1. argv - Argument Vector*
It stores what you type in terminal. It is an array of strings.
Ex: if you type `./exp6 50`, argv[0] = ./exp6, argv[1] = 50

*2. argc - Argument Count*
Number of words you typed in terminal.
Ex: `./exp6 50` has argc = 2

*3. atoi() - ASCII to Integer*
Converts string to integer. Converts "50" string into int 50.
Needs header: `#include <stdlib.h>`
Ex: `int n = atoi(argv[1]);`

*4. sleep()*
Pauses the program for given seconds.
Ex: `sleep(1);` - pauses for 1 second
Needs header: `#include <unistd.h>`

*5. malloc() - Memory Allocation*
Used to allocate memory during runtime (dynamic memory).
Ex: `malloc(1024)` allocates 1024 bytes
Needs header: `#include <stdlib.h>`

*6. #include <stdlib.h>*
Header file for malloc(), free(), atoi()

*7. #include <unistd.h>*
Header file for sleep() function

*8. free -h*
Shows how much RAM is used and how much is free.
`-h` means human-readable format (shows in MB/GB, not bytes)

*9. watch -n 1 free -h*
Runs a particular command again and again automatically.
`watch` will run `free -h` every 1 second so you can observe memory change in real time.
To exit: Press `Ctrl + C`

*10. gcc exp6.c -o exp6*
Compiles C program.

*11. time ./exp6 50*
Measures execution time and runs the program with argument 50.

*How it works in this Exp:*
You allocate memory using malloc in a loop and observe in other terminal with `watch -n 1 free -h` that free memory decreases.

