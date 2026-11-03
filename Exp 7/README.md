AIM: Write a CPU bound C program and I/O bound C program and observe the effect of their CPU share using top command.THEORY / All Commands - In Same Way as 5:• CPU bound -
A process that is limited by the speed of the CPU and spends the majority of its execution time in the CPU burst time. It keeps CPU busy.• I/O bound -
A process that is limited by the speed of I/O devices and spends the majority of its execution time waiting for I/O operations to complete.• pgrep -a cpu_bound -
It lists all running processes with name cpu_bound along with their PID. Used to find PID of your program to monitor in top.• top -p <PID> -
This successfully monitors only PID. Shows only that particular process, not all. Used to see CPU % of your program.• %CPU 90.7% -
Process is using almost 1 full CPU core. In CPU bound it shows 90-100%, in I/O bound it shows very low like 0-2%.• S=R -
Status Running. Process is always running. In top, S column shows state. CPU bound = R, I/O bound = S (sleeping).• FILE *fp -
Creates a file pointer to handle files. Used in I/O bound program to open/write file.• fopen() -
Open the file. 
Ex: fopen("file.txt", "w")• fclose() -
Close the file. After finishing file work.• fprintf() -
Write text inside " " into file. Writes data into file for I/O operation.• "w" mode -
Check whether the file existed, if existed, empty it, if not create another file. Used to create new file every time.• gcc file.c -o cpu_bound -
Compiles C program into executable.• ./cpu_bound & -
