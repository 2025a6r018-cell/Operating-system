

*EXP. No. 4(a)(b)(c)*

*AIM:* 
(a) To determine the period for which a specific user is working
(b) To display lines between start and end line numbers
(c) To delete lines containing a specified word

*THEORY / All Commands:*

*• who -*
Displays list of all users currently logged in with login time.
We need this to find for how long a user is working.

*• awk -*
Powerful text processing filter. It divides each line into columns $1, $2, $3...
`$1` is username, `$3,$4` is login time and date.

*• awk -v -*
`-v` is used to pass a shell variable into awk.
Ex: `awk -v u="$user"` - passes shell variable $user as u inside awk.

*• $1==u {print $3,$4; exit} -*
Condition inside awk. If first column equals user, print login time and exit.

*• read -p -*
Reads input from keyboard with a message.
`read -p "Enter username: " user`

*• sed -*
Stream Editor, used for editing and printing files.

*• sed -n 'start,end p' -*
`-n` suppresses auto-print. `p` prints only lines from start to end.
Ex: `sed -n '5,10p' file.txt` - prints line 5 to 10.

*• sed -i "/word/d" -*
`-i` means in-place, makes changes permanent in file.
`/word/d` - deletes all lines containing that word.

*• shift -*
Shifts all arguments to left by one position.
So $1 (word) is removed and $2,$3 become new $1,$2 which are filenames.

*• $@ -*
Represents all filenames passed as arguments.

*• $# -*
Counts total number of arguments passed.
Used to check if user gave filename or not.

*• [ -f "$file" ] -*
Checks if file exists and is a regular file before processing.

*• chmod +x file.sh -*
Makes shell script executable.

