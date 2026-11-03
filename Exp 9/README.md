

*AIM:* Write a program in C that creates a child process, prints termination of the child and lists its PID.

*THEORY / All Commands - In Same Way as 5:*

*• PID -*
Unique ID given by OS to every Process. Har process ka alag number hota hai.

*• Parent Process -*
Original process that calls fork() to create child. Jo pehle se chal raha hai.

*• Child Process -*
New process created by Parent. It is copy of parent but has different PID.

*• fork() -*
System call used to create child. It returns 0 in child process and PID of child in parent process. If fail, returns -1.
Needs: `#include <unistd.h>`

*• pid_t -*
A datatype for pid functions. PID store karne ke liye use hota hai.

*• getpid() -*
Returns PID of the process calling it. Apna khud ka PID batata hai.

*• getppid() -*
Returns PID of Parent of calling process. Apne parent ka PID batata hai.

*• wait() -*
Return the PID of CHILD that is terminated, list which child is reaped. Parent wait karta hai child khatam hone tak.

*• #include <sys/wait.h> -*
For wait() function. Wait use karne ke liye ye header lagana padta hai.

