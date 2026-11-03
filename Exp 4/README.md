1. who
Shows list of all users currently logged in with their login time and terminal
.2. read
Reads input from keyboard.
read -p "message" var - Displays message and stores input in variable.3. awk
A text processing tool that divides each line into columns ($1, $2, $3...).
Example: awk '{print $1}' prints first column.4. awk -v
Used to pass a shell variable into awk.
Example: awk -v u="$user" '$1==u' - passes user variable as u.5. sed
Stream Editor used for editing text/files.6. sed -n
-n suppresses automatic printing. Prints only specified lines.
sed -n '5,10p' file - prints lines 5 to 10.7. sed -i
-i makes changes permanent in the file (in-place editing).
sed -i "/word/d" file - deletes lines containing word permanently.8. shift
Shifts all positional arguments to left by one.
After shift, $2 becomes $1, $3 becomes $2, etc. Used to separate word from filenames.9. $#
Counts total number of arguments passed.10. $@
Represents all arguments passed as a list.11. $1, $2, $3
Positional parameters. $1 is first argument, $2 is second.12. [ -f file ]
Checks if file exists and is a regular file.13. [ -z string ]
Checks if string is empty.14. grep -w
Searches for exact word.15. exit
Exits the script or awk program.16. chmod +x
Makes a file executable.Copy this directly in your practical file under "Commands Used" heading.





