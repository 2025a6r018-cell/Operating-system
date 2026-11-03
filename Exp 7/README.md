

*EXP. No. 9 - CPU Bound & I/O Bound*

*AIM:* To run CPU bound & I/O bound C programs and check CPU % using top.

*THEORY:*

*1. CPU bound -*
Program jo CPU ka pura use karta hai. Calculation karta rehta hai.

*2. I/O bound -*
Program jo file / disk ka wait karta hai. CPU free rehta hai.

*All Commands:*

*• pgrep -a cpu_bound -*
PID dhoondhne ke liye. Program ka number deta hai.

*• top -p <PID> -*
Sirf uss PID ka CPU usage dekhta hai.

*• %CPU -*
Kitna CPU use ho raha hai. CPU bound = 90%+, I/O bound = 0-1%

*• S -*
Status. R = Running, S = Sleeping.

*• FILE *fp -*
File pointer. File handle karne ke liye.

*• fopen / fclose -*
File open / close karna.

*• fprintf -*
File me likhna.

*• gcc & ./a.out & -*
Compile & background me run karna. `&` se terminal free rahega top chalane ke liye.

---

*Result:*
CPU bound takes 99% CPU. I/O bound takes 0% CPU.

