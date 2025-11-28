# 🛠️ DevOps Tiny Steps: 600 Exercises for Complete Beginners

A complete, gradual learning path designed for absolute beginners with zero knowledge. Each exercise teaches exactly ONE concept with clear explanations. All exercises are local/on-premise - no cloud required.

## How to Use This Guide
- ✅ = Complete
- 📝 = In Progress  
- ⭐ = Important Concept
- 🎯 = Practice This Multiple Times
- ⚠️ = Be Careful Here

---

## 🌟 PHASE 1: Linux Fundamentals (Exercises 1-80)

### Week 1: Your First Steps with the Terminal

**Exercise 1: Open the Terminal** ⭐✅  
**Goal:** Access the command line for the first time  
**Task:** Open a terminal on your Linux system (or WSL on Windows)  
**Concept:** The terminal is where DevOps magic happens  
**Help:** Press `Ctrl+Alt+T` on Ubuntu, or search for "Terminal"

**Exercise 2: Who Am I?** ✅  
**Goal:** Find out your current username  
**Task:** Type `whoami` and press Enter  
**Concept:** The `whoami` command shows your username  
**Help:** You should see your username printed

**Exercise 3: Where Am I?** ⭐✅  
**Goal:** Find your current location in the file system  
**Task:** Type `pwd` and press Enter  
**Concept:** `pwd` = Print Working Directory  
**Help:** You'll likely see `/home/yourusername`

**Exercise 4: What's Here?** ⭐✅  
**Goal:** See files and folders in current directory  
**Task:** Type `ls` and press Enter  
**Concept:** `ls` = List directory contents  
**Help:** You'll see files and folders listed

**Exercise 5: List with Details** ✅
**Goal:** See more information about files  
**Task:** Type `ls -l` and press Enter  
**Concept:** `-l` flag shows long format with details  
**Help:** You'll see permissions, owner, size, date

**Exercise 6: Show Hidden Files** ✅ 
**Goal:** See files that start with a dot  
**Task:** Type `ls -a` and press Enter  
**Concept:** Hidden files start with `.` (like `.bashrc`)  
**Help:** `-a` means "all" including hidden

**Exercise 7: Combine Flags** ✅ 
**Goal:** Use multiple options together  
**Task:** Type `ls -la` and press Enter  
**Concept:** Flags can be combined  
**Help:** Shows all files in long format

**Exercise 8: Human Readable Sizes** ✅ 
**Goal:** See file sizes in KB, MB, GB  
**Task:** Type `ls -lh` and press Enter  
**Concept:** `-h` = human readable  
**Help:** Instead of bytes, you'll see "4.0K", "1.2M", etc.

**Exercise 9: Clear the Screen** ✅
**Goal:** Clean up your terminal  
**Task:** Type `clear` or press `Ctrl+L`  
**Concept:** Clears terminal output  
**Help:** Your prompt will be at the top

**Exercise 10: Your First Directory** ⭐✅  
**Goal:** Create a new folder  
**Task:** Type `mkdir devops-practice`  
**Concept:** `mkdir` = Make Directory  
**Help:** This creates a folder called "devops-practice"

---

### Week 2: Navigation & Basic Commands

**Exercise 11: Change Directory** ⭐✅  
**Goal:** Move into a folder  
**Task:** Type `cd devops-practice`  
**Concept:** `cd` = Change Directory  
**Help:** Use `pwd` to confirm you moved

**Exercise 12: Go Back One Level** ✅ 
**Goal:** Move to parent directory  
**Task:** Type `cd ..`  
**Concept:** `..` means parent directory  
**Help:** You should be back where you started

**Exercise 13: Go Home** ⭐✅  
**Goal:** Return to your home directory  
**Task:** Type `cd ~` or just `cd`  
**Concept:** `~` is shortcut for home directory  
**Help:** `pwd` should show `/home/yourusername`

**Exercise 14: Absolute vs Relative Paths** ✅ 
**Goal:** Understand path types  
**Task:** Try `cd /home` then `cd ~`  
**Concept:** Absolute starts with `/`, relative doesn't  
**Help:** `/home` is absolute, `devops-practice` is relative

**Exercise 15: Create Nested Directories** ✅ 
**Goal:** Create folders inside folders  
**Task:** `mkdir -p projects/web/frontend`  
**Concept:** `-p` creates parent directories as needed  
**Help:** Creates projects, web inside it, frontend inside that

**Exercise 16: Create an Empty File** ⭐✅  
**Goal:** Make a new empty file  
**Task:** `touch myfile.txt`  
**Concept:** `touch` creates empty files  
**Help:** Use `ls` to verify it exists

**Exercise 17: Create Multiple Files**  ✅
**Goal:** Create several files at once  
**Task:** `touch file1.txt file2.txt file3.txt`  
**Concept:** Commands can take multiple arguments  
**Help:** Three files created with one command

**Exercise 18: View File Contents** ⭐✅  
**Goal:** Read what's in a file  
**Task:** `cat /etc/hostname`  
**Concept:** `cat` displays file contents  
**Help:** Shows your computer's hostname

**Exercise 19: Create File with Content** ✅
**Goal:** Write text to a file  
**Task:** `echo "Hello DevOps" > hello.txt`  
**Concept:** `>` redirects output to file  
**Help:** `cat hello.txt` to verify

**Exercise 20: Append to File** ✅ 
**Goal:** Add more text without overwriting  
**Task:** `echo "Learning Linux" >> hello.txt`  
**Concept:** `>>` appends to file  
**Help:** `cat hello.txt` shows both lines

---

### Week 3: File Operations

**Exercise 21: Copy a File** ⭐✅  
**Goal:** Duplicate a file  
**Task:** `cp hello.txt hello-backup.txt`  
**Concept:** `cp` = Copy  
**Help:** Now you have two files with same content

**Exercise 22: Copy to Directory**✅  
**Goal:** Copy file into a folder  
**Task:** `cp hello.txt devops-practice/`  
**Concept:** Destination can be a directory  
**Help:** File is now in both locations

**Exercise 23: Copy Directory** ⭐✅  
**Goal:** Copy an entire folder  
**Task:** `cp -r devops-practice backup-folder`  
**Concept:** `-r` = recursive (needed for directories)  
**Help:** Without `-r`, copying directories fails

**Exercise 24: Move a File** ⭐✅  
**Goal:** Move file to new location  
**Task:** `mv hello.txt devops-practice/`  
**Concept:** `mv` = Move  
**Help:** File is no longer in original location

**Exercise 25: Rename a File**✅  
**Goal:** Change file name  
**Task:** `mv hello-backup.txt greeting.txt`  
**Concept:** `mv` also renames files  
**Help:** Same command, just different name

**Exercise 26: Rename a Directory**✅  
**Goal:** Change folder name  
**Task:** `mv backup-folder archive`  
**Concept:** `mv` works on directories too  
**Help:** No `-r` needed for moving directories

**Exercise 27: Remove a File** ⭐ ⚠️✅  
**Goal:** Delete a file  
**Task:** `rm greeting.txt`  
**Concept:** `rm` = Remove (PERMANENT - no trash!)  
**Warning:** There is no undo! Double-check before removing

**Exercise 28: Remove Empty Directory**✅  
**Goal:** Delete an empty folder  
**Task:** `rmdir archive`  
**Concept:** `rmdir` only removes empty directories  
**Help:** If directory has files, this will fail

**Exercise 29: Remove Directory with Contents** ⚠️✅  
**Goal:** Delete folder and everything inside  
**Task:** `rm -r devops-practice`  
**Concept:** `-r` removes recursively  
**Warning:** Very dangerous! Always double-check path

**Exercise 30: Safe Delete Practice** 🎯✅  
**Goal:** Confirm before deleting  
**Task:** `rm -i file1.txt`  
**Concept:** `-i` asks for confirmation  
**Help:** Type `y` for yes, `n` for no

---

### Week 4: Viewing & Editing Files

**Exercise 31: View Long Files** ⭐✅  
**Goal:** Read files that don't fit on screen  
**Task:** `less /etc/services`  
**Concept:** `less` allows scrolling through files  
**Help:** Press `q` to quit, arrows to scroll

**Exercise 32: View First Lines**✅  
**Goal:** See beginning of a file  
**Task:** `head /etc/passwd`  
**Concept:** `head` shows first 10 lines  
**Help:** Default is 10 lines

**Exercise 33: View Last Lines** ⭐✅  
**Goal:** See end of a file  
**Task:** `tail /etc/passwd`  
**Concept:** `tail` shows last 10 lines  
**Help:** Very useful for log files!

**Exercise 34: Specify Number of Lines**✅  
**Goal:** Control how many lines to show  
**Task:** `head -n 5 /etc/passwd`  
**Concept:** `-n` specifies line count  
**Help:** Shows first 5 lines

**Exercise 35: Follow Log File** ⭐✅ 
**Goal:** Watch file updates in real-time  
**Task:** `tail -f /var/log/syslog`  
**Concept:** `-f` = follow (updates live)  
**Help:** Press `Ctrl+C` to stop

**Exercise 36: Word Count** ✅ 
**Goal:** Count lines, words, characters  
**Task:** `wc /etc/passwd`  
**Concept:** `wc` = Word Count  
**Help:** Shows: lines, words, characters

**Exercise 37: Count Lines Only** ✅ 
**Goal:** Get just the line count  
**Task:** `wc -l /etc/passwd`  
**Concept:** `-l` = lines only  
**Help:** Useful for counting entries

**Exercise 38: Nano Editor** ⭐✅ 
**Goal:** Edit a file with simple editor  
**Task:** `nano myfile.txt`, type text, `Ctrl+O` to save, `Ctrl+X` to exit  
**Concept:** `nano` is beginner-friendly editor  
**Help:** Commands shown at bottom of screen

**Exercise 39: Vim Basics - Open and Quit** ⭐✅  
**Goal:** Learn to safely exit vim  
**Task:** `vim myfile.txt`, press `Esc`, type `:q!`, press Enter  
**Concept:** Vim has modes; `:q!` quits without saving  
**Help:** `:q!` = quit, discard changes (very important!)

**Exercise 40: Vim - Insert Mode**✅  
**Goal:** Type text in vim  
**Task:** Open vim, press `i`, type text, press `Esc`, type `:wq`, Enter  
**Concept:** `i` enters insert mode, `Esc` exits it  
**Help:** `:wq` = write and quit (save and exit)

---

### Week 5: Finding Things

**Exercise 41: Find Files by Name** ⭐✅  
**Goal:** Search for files  
**Task:** `find /home -name "*.txt"`  
**Concept:** `find` searches filesystem  
**Help:** `*.txt` matches all .txt files

**Exercise 42: Find Case Insensitive**✅  
**Goal:** Search ignoring uppercase/lowercase  
**Task:** `find /home -iname "*.TXT"`  
**Concept:** `-iname` ignores case  
**Help:** Matches .txt, .TXT, .Txt, etc.

**Exercise 43: Find Directories Only**✅  
**Goal:** Search only for folders  
**Task:** `find /home -type d -name "project*"`  
**Concept:** `-type d` = directories only  
**Help:** `-type f` would be files only

**Exercise 44: Find by Size**✅  
**Goal:** Find large files  
**Task:** `find /home -size +10M`  
**Concept:** `+10M` = larger than 10 megabytes  
**Help:** `-10M` would be smaller than 10MB

**Exercise 45: Search Inside Files** ⭐✅  
**Goal:** Find text within files  
**Task:** `grep "hello" myfile.txt`  
**Concept:** `grep` searches file contents  
**Help:** Shows lines containing "hello"

**Exercise 46: Case Insensitive Search**  
**Goal:** Search ignoring case  
**Task:** `grep -i "HELLO" myfile.txt`  
**Concept:** `-i` = ignore case  
**Help:** Matches hello, HELLO, Hello, etc.

**Exercise 47: Search Recursively** ⭐  
**Goal:** Search all files in directory tree  
**Task:** `grep -r "error" /var/log`  
**Concept:** `-r` searches subdirectories too  
**Help:** Very useful for finding errors in logs

**Exercise 48: Show Line Numbers**  
**Goal:** Know where matches are  
**Task:** `grep -n "hello" myfile.txt`  
**Concept:** `-n` shows line numbers  
**Help:** Output: `3:hello world` (line 3)

**Exercise 49: Count Matches**  
**Goal:** How many times text appears  
**Task:** `grep -c "the" myfile.txt`  
**Concept:** `-c` = count matching lines  
**Help:** Returns a number

**Exercise 50: Find Command Location** ⭐  
**Goal:** Where is a command installed  
**Task:** `which python`  
**Concept:** `which` shows command path  
**Help:** Shows `/usr/bin/python` or similar

---

### Week 6: Pipes & Redirection

**Exercise 51: Pipe Output** ⭐  
**Goal:** Send output from one command to another  
**Task:** `ls -la | less`  
**Concept:** `|` (pipe) connects commands  
**Help:** Long listing paginated by less

**Exercise 52: Chain Multiple Pipes**  
**Goal:** Create command pipeline  
**Task:** `cat /etc/passwd | grep "bash" | wc -l`  
**Concept:** Multiple pipes = powerful filtering  
**Help:** Counts users with bash shell

**Exercise 53: Save Output to File** ⭐  
**Goal:** Redirect output to file  
**Task:** `ls -la > filelist.txt`  
**Concept:** `>` redirects stdout to file  
**Help:** Overwrites if file exists

**Exercise 54: Append Output**  
**Goal:** Add to file without overwriting  
**Task:** `echo "new entry" >> filelist.txt`  
**Concept:** `>>` appends to file  
**Help:** Adds to end of file

**Exercise 55: Redirect Errors**  
**Goal:** Save error messages separately  
**Task:** `ls /nonexistent 2> errors.txt`  
**Concept:** `2>` redirects stderr (errors)  
**Help:** `2` is the error file descriptor

**Exercise 56: Redirect Both**  
**Goal:** Save output and errors  
**Task:** `ls /home /nonexistent > output.txt 2>&1`  
**Concept:** `2>&1` sends errors to same place as output  
**Help:** Both streams go to output.txt

**Exercise 57: Discard Output**  
**Goal:** Run command silently  
**Task:** `ls > /dev/null`  
**Concept:** `/dev/null` is the "black hole"  
**Help:** Output disappears

**Exercise 58: Sort Output** ⭐  
**Goal:** Arrange lines alphabetically  
**Task:** `cat /etc/passwd | sort`  
**Concept:** `sort` arranges lines in order  
**Help:** Alphabetical by default

**Exercise 59: Sort Numerically**  
**Goal:** Sort by number  
**Task:** Create file with numbers, use `sort -n`  
**Concept:** `-n` = numeric sort  
**Help:** Otherwise 10 comes before 2

**Exercise 60: Remove Duplicates** ⭐  
**Goal:** Keep only unique lines  
**Task:** `sort myfile.txt | uniq`  
**Concept:** `uniq` removes adjacent duplicates  
**Help:** Must sort first!

---

### Week 7: Permissions & Ownership

**Exercise 61: View Permissions** ⭐  
**Goal:** Understand file permissions  
**Task:** `ls -l` and look at first column  
**Concept:** `-rwxr-xr-x` format  
**Help:** r=read, w=write, x=execute

**Exercise 62: Understand Permission Groups**  
**Goal:** Know who permissions apply to  
**Task:** Study `-rwxr-xr-x` format  
**Concept:** Owner, Group, Others (3 sets of 3)  
**Help:** First 3 = owner, next 3 = group, last 3 = others

**Exercise 63: Change Permissions - Symbolic** ⭐  
**Goal:** Modify file permissions  
**Task:** `chmod u+x script.sh`  
**Concept:** u=user, g=group, o=others, a=all  
**Help:** `+` adds, `-` removes permission

**Exercise 64: Make File Executable**  
**Goal:** Allow file to run as program  
**Task:** `chmod +x myscript.sh`  
**Concept:** `+x` adds execute for all  
**Help:** Now you can run `./myscript.sh`

**Exercise 65: Remove Write Permission**  
**Goal:** Protect file from changes  
**Task:** `chmod -w important.txt`  
**Concept:** `-w` removes write permission  
**Help:** File becomes read-only

**Exercise 66: Numeric Permissions** ⭐  
**Goal:** Use number-based permissions  
**Task:** `chmod 755 script.sh`  
**Concept:** 7=rwx, 5=r-x, 4=r--, 0=---  
**Help:** 755 = owner:all, group:read+exec, others:read+exec

**Exercise 67: Common Permission Numbers** 🎯  
**Goal:** Memorize common permissions  
**Task:** Practice 644, 755, 700, 600  
**Concept:** 644=file, 755=script, 700=private dir, 600=secrets  
**Help:** These cover most use cases

**Exercise 68: View File Owner**  
**Goal:** See who owns a file  
**Task:** `ls -l` and look at 3rd and 4th columns  
**Concept:** Shows owner username and group  
**Help:** Format: owner group

**Exercise 69: Change Owner** ⭐  
**Goal:** Transfer file ownership  
**Task:** `sudo chown newuser myfile.txt`  
**Concept:** `chown` = change owner  
**Help:** Requires root/sudo usually

**Exercise 70: Change Group**  
**Goal:** Modify file's group  
**Task:** `sudo chgrp newgroup myfile.txt`  
**Concept:** `chgrp` = change group  
**Help:** Or use `chown :groupname file`

---

### Week 8: Users, Groups & Processes

**Exercise 71: List All Users**  
**Goal:** See system users  
**Task:** `cat /etc/passwd`  
**Concept:** User info stored in /etc/passwd  
**Help:** Each line is one user

**Exercise 72: Current User Info**  
**Goal:** See your user details  
**Task:** `id`  
**Concept:** Shows uid, gid, and groups  
**Help:** uid = user id, gid = group id

**Exercise 73: See Your Groups**  
**Goal:** List groups you belong to  
**Task:** `groups`  
**Concept:** Users can be in multiple groups  
**Help:** Affects what files you can access

**Exercise 74: Switch User** ⭐  
**Goal:** Become another user  
**Task:** `su - username`  
**Concept:** `su` = switch user  
**Help:** Need that user's password

**Exercise 75: Sudo - Run as Root** ⭐  
**Goal:** Execute command with admin rights  
**Task:** `sudo whoami`  
**Concept:** `sudo` runs command as root  
**Help:** Should output "root"

**Exercise 76: View Running Processes** ⭐  
**Goal:** See what's running  
**Task:** `ps aux`  
**Concept:** `ps` shows process status  
**Help:** `aux` shows all users' processes

**Exercise 77: Interactive Process View**  
**Goal:** Monitor processes in real-time  
**Task:** `top`  
**Concept:** `top` shows live process info  
**Help:** Press `q` to quit

**Exercise 78: Better Process Viewer**  
**Goal:** Use friendlier process monitor  
**Task:** `htop` (install if needed)  
**Concept:** `htop` is enhanced `top`  
**Help:** `sudo apt install htop` to install

**Exercise 79: Find Process by Name** ⭐  
**Goal:** Search for specific process  
**Task:** `ps aux | grep nginx`  
**Concept:** Combine ps with grep  
**Help:** Shows only matching processes

**Exercise 80: Kill a Process** ⭐ ⚠️  
**Goal:** Stop a running process  
**Task:** `kill PID` (replace PID with actual number)  
**Concept:** Sends termination signal  
**Warning:** Don't kill system processes!

---

## 🔧 PHASE 2: Shell Scripting (Exercises 81-140)

### Week 9: Your First Scripts

**Exercise 81: Create First Script** ⭐  
**Goal:** Write your first shell script  
**Task:** Create `hello.sh` with `#!/bin/bash` and `echo "Hello DevOps"`  
**Concept:** Scripts are text files with commands  
**Help:** First line (shebang) tells system which interpreter

**Exercise 82: Make Script Executable**  
**Goal:** Allow script to run  
**Task:** `chmod +x hello.sh`  
**Concept:** Scripts need execute permission  
**Help:** Without this, you'll get "Permission denied"

**Exercise 83: Run Your Script** ⭐  
**Goal:** Execute the script  
**Task:** `./hello.sh`  
**Concept:** `./` means "current directory"  
**Help:** You should see "Hello DevOps"

**Exercise 84: Run with Bash**  
**Goal:** Alternative way to run scripts  
**Task:** `bash hello.sh`  
**Concept:** Explicitly specify interpreter  
**Help:** Works even without execute permission

**Exercise 85: Script with Multiple Commands**  
**Goal:** Run several commands in sequence  
**Task:** Script with `echo`, `date`, and `whoami`  
**Concept:** Commands run top to bottom  
**Help:** Each command on its own line

**Exercise 86: Add Comments** ⭐  
**Goal:** Document your script  
**Task:** Add `# This is a comment` lines  
**Concept:** Comments explain code, ignored when running  
**Help:** Start line with `#`

**Exercise 87: Variables in Scripts** ⭐  
**Goal:** Store and use values  
**Task:** `NAME="DevOps"` then `echo "Hello $NAME"`  
**Concept:** Variables store data  
**Help:** No spaces around `=`!

**Exercise 88: Read User Input**  
**Goal:** Get input from user  
**Task:** `read -p "Enter name: " NAME`  
**Concept:** `read` gets user input  
**Help:** `-p` shows prompt message

**Exercise 89: Command Substitution** ⭐  
**Goal:** Store command output in variable  
**Task:** `TODAY=$(date)` then `echo "Today is $TODAY"`  
**Concept:** `$()` runs command and captures output  
**Help:** Also works with backticks: \`date\`

**Exercise 90: Environment Variables**  
**Goal:** Access system variables  
**Task:** `echo "Home is $HOME, User is $USER"`  
**Concept:** System provides useful variables  
**Help:** `env` shows all environment variables

---

### Week 10: Script Logic

**Exercise 91: If Statement** ⭐  
**Goal:** Make decisions in scripts  
**Task:** `if [ $NUM -gt 10 ]; then echo "Big"; fi`  
**Concept:** `if` checks conditions  
**Help:** `-gt` = greater than

**Exercise 92: If-Else**  
**Goal:** Two possible outcomes  
**Task:** Add `else echo "Small"` before `fi`  
**Concept:** `else` handles false condition  
**Help:** Don't forget `fi` at the end

**Exercise 93: Comparison Operators** 🎯  
**Goal:** Learn all comparison types  
**Task:** Practice `-eq`, `-ne`, `-lt`, `-le`, `-gt`, `-ge`  
**Concept:** eq=equal, ne=not equal, lt=less than, etc.  
**Help:** These work with numbers

**Exercise 94: String Comparison**  
**Goal:** Compare text values  
**Task:** `if [ "$NAME" = "admin" ]; then ...`  
**Concept:** Use `=` and `!=` for strings  
**Help:** Always quote variables!

**Exercise 95: Check If File Exists** ⭐  
**Goal:** Test for file existence  
**Task:** `if [ -f myfile.txt ]; then echo "exists"; fi`  
**Concept:** `-f` checks if file exists  
**Help:** `-d` checks for directory

**Exercise 96: Check If Directory Exists**  
**Goal:** Test for directory  
**Task:** `if [ -d /tmp ]; then echo "directory exists"; fi`  
**Concept:** `-d` = is a directory  
**Help:** Useful before mkdir

**Exercise 97: Logical AND**  
**Goal:** Multiple conditions must be true  
**Task:** `if [ $A -gt 5 ] && [ $B -lt 10 ]; then ...`  
**Concept:** `&&` = both conditions true  
**Help:** Can also use `-a` inside single brackets

**Exercise 98: Logical OR**  
**Goal:** Either condition true  
**Task:** `if [ $A -eq 1 ] || [ $A -eq 2 ]; then ...`  
**Concept:** `||` = at least one true  
**Help:** Can also use `-o` inside single brackets

**Exercise 99: Elif for Multiple Conditions**  
**Goal:** Check multiple options  
**Task:** `if ... elif ... elif ... else ... fi`  
**Concept:** `elif` = else if  
**Help:** Checks conditions in order

**Exercise 100: Case Statement** ⭐  
**Goal:** Match multiple patterns  
**Task:** `case $VAR in pattern1) ... ;; pattern2) ... ;; esac`  
**Concept:** `case` is like switch in other languages  
**Help:** End each pattern with `;;`

---

### Week 11: Loops

**Exercise 101: For Loop - List** ⭐  
**Goal:** Repeat for each item  
**Task:** `for i in 1 2 3 4 5; do echo $i; done`  
**Concept:** `for` iterates over list  
**Help:** `do` starts body, `done` ends it

**Exercise 102: For Loop - Range**  
**Goal:** Loop through number range  
**Task:** `for i in {1..10}; do echo $i; done`  
**Concept:** `{1..10}` generates 1 to 10  
**Help:** Bash 3+ feature

**Exercise 103: For Loop - Files** ⭐  
**Goal:** Process multiple files  
**Task:** `for f in *.txt; do echo "File: $f"; done`  
**Concept:** Wildcards in for loops  
**Help:** Very common pattern!

**Exercise 104: C-style For Loop**  
**Goal:** Traditional for loop  
**Task:** `for ((i=0; i<10; i++)); do echo $i; done`  
**Concept:** Initialize, condition, increment  
**Help:** Double parentheses for arithmetic

**Exercise 105: While Loop** ⭐  
**Goal:** Loop while condition is true  
**Task:** `while [ $COUNT -lt 10 ]; do echo $COUNT; ((COUNT++)); done`  
**Concept:** `while` repeats until condition false  
**Help:** Don't forget to update counter!

**Exercise 106: Infinite Loop**  
**Goal:** Loop forever (until break)  
**Task:** `while true; do echo "Running"; sleep 1; done`  
**Concept:** `while true` never ends  
**Help:** Press `Ctrl+C` to stop

**Exercise 107: Break Statement**  
**Goal:** Exit loop early  
**Task:** Add `if [ $i -eq 5 ]; then break; fi` inside loop  
**Concept:** `break` exits the loop immediately  
**Help:** Useful for search loops

**Exercise 108: Continue Statement**  
**Goal:** Skip to next iteration  
**Task:** `if [ $i -eq 5 ]; then continue; fi`  
**Concept:** `continue` skips rest of current iteration  
**Help:** Loop continues with next item

**Exercise 109: Read File Line by Line** ⭐  
**Goal:** Process each line of a file  
**Task:** `while read line; do echo "$line"; done < file.txt`  
**Concept:** `read` with input redirection  
**Help:** Very common for log processing

**Exercise 110: Loop with Counter**  
**Goal:** Track iterations  
**Task:** Count lines while reading file  
**Concept:** Combine while loop with counter  
**Help:** `((COUNT++))` increments counter

---

### Week 12: Functions & Arguments

**Exercise 111: Script Arguments** ⭐  
**Goal:** Accept command line arguments  
**Task:** Access `$1`, `$2`, `$3` in script  
**Concept:** `$1` is first argument, `$2` is second, etc.  
**Help:** `$0` is the script name itself

**Exercise 112: Number of Arguments**  
**Goal:** Know how many arguments passed  
**Task:** Use `$#` to get count  
**Concept:** `$#` = argument count  
**Help:** Useful for validation

**Exercise 113: All Arguments**  
**Goal:** Access all arguments at once  
**Task:** Use `$@` or `$*`  
**Concept:** `$@` = all arguments as separate strings  
**Help:** `$*` joins them with spaces

**Exercise 114: Check Required Arguments**  
**Goal:** Validate input  
**Task:** `if [ $# -lt 1 ]; then echo "Usage: ..."; exit 1; fi`  
**Concept:** Exit if arguments missing  
**Help:** `exit 1` indicates error

**Exercise 115: Define a Function** ⭐  
**Goal:** Create reusable code block  
**Task:** `greet() { echo "Hello $1"; }`  
**Concept:** Functions group commands  
**Help:** Call with `greet "World"`

**Exercise 116: Function with Return Value**  
**Goal:** Return status from function  
**Task:** `return 0` for success, `return 1` for failure  
**Concept:** Return codes indicate success/failure  
**Help:** Check with `$?` after calling

**Exercise 117: Function with Output**  
**Goal:** Get output from function  
**Task:** `result=$(my_function)`  
**Concept:** Capture function's echo output  
**Help:** More flexible than return codes

**Exercise 118: Local Variables**  
**Goal:** Variables scoped to function  
**Task:** `local NAME="value"` inside function  
**Concept:** `local` prevents variable leaking  
**Help:** Good practice in functions

**Exercise 119: Function Library**  
**Goal:** Reuse functions across scripts  
**Task:** `source functions.sh` or `. functions.sh`  
**Concept:** Source includes another script  
**Help:** Common for shared utilities

**Exercise 120: Exit Codes** ⭐  
**Goal:** Handle script success/failure  
**Task:** `exit 0` for success, `exit 1` for error  
**Concept:** Exit codes tell caller what happened  
**Help:** `$?` holds last command's exit code

---

### Week 13: Text Processing

**Exercise 121: Cut Command** ⭐  
**Goal:** Extract columns from text  
**Task:** `echo "a:b:c" | cut -d: -f2`  
**Concept:** `cut` extracts fields  
**Help:** `-d` delimiter, `-f` field number

**Exercise 122: Cut Multiple Fields**  
**Goal:** Extract several columns  
**Task:** `cut -d: -f1,3 /etc/passwd`  
**Concept:** Comma separates field numbers  
**Help:** Gets username and UID

**Exercise 123: Awk Basics** ⭐  
**Goal:** Powerful text processing  
**Task:** `echo "hello world" | awk '{print $2}'`  
**Concept:** `awk` splits on whitespace by default  
**Help:** `$1` first field, `$2` second, etc.

**Exercise 124: Awk Field Separator**  
**Goal:** Use custom delimiter  
**Task:** `awk -F: '{print $1}' /etc/passwd`  
**Concept:** `-F` sets field separator  
**Help:** Gets all usernames

**Exercise 125: Awk with Conditions**  
**Goal:** Filter with awk  
**Task:** `awk '$3 > 1000 {print $1}' /etc/passwd`  
**Concept:** Condition before action  
**Help:** Print username if UID > 1000

**Exercise 126: Sed Basics** ⭐  
**Goal:** Stream editor for text  
**Task:** `echo "hello" | sed 's/hello/goodbye/'`  
**Concept:** `s/old/new/` substitutes text  
**Help:** `sed` = stream editor

**Exercise 127: Sed Replace All**  
**Goal:** Replace all occurrences  
**Task:** `echo "ha ha ha" | sed 's/ha/ho/g'`  
**Concept:** `g` flag = global (all matches)  
**Help:** Without `g`, only first match replaced

**Exercise 128: Sed Edit File** ⭐  
**Goal:** Modify file in place  
**Task:** `sed -i 's/old/new/g' file.txt`  
**Concept:** `-i` edits file directly  
**Help:** Be careful! Makes permanent changes

**Exercise 129: Sed Delete Lines**  
**Goal:** Remove lines matching pattern  
**Task:** `sed '/pattern/d' file.txt`  
**Concept:** `d` command deletes line  
**Help:** Useful for cleaning log files

**Exercise 130: Tr Command**  
**Goal:** Translate characters  
**Task:** `echo "hello" | tr 'a-z' 'A-Z'`  
**Concept:** `tr` translates/replaces characters  
**Help:** Converts to uppercase

---

### Week 14: Practical Scripts

**Exercise 131: Backup Script** ⭐ 📝  
**Goal:** Create automatic backup  
**Task:** Script that copies directory with timestamp  
**Concept:** Combine date, mkdir, cp  
**Help:** `DATE=$(date +%Y%m%d)` for timestamp

**Exercise 132: Log Rotation Script**  
**Goal:** Manage log file size  
**Task:** Rename log, create new empty one  
**Concept:** Basic log management  
**Help:** `mv log.txt log.txt.1; touch log.txt`

**Exercise 133: Disk Usage Alert**  
**Goal:** Check disk space  
**Task:** Script that warns if disk > 80% full  
**Concept:** `df` for disk usage  
**Help:** `df -h | grep '/' | awk '{print $5}'`

**Exercise 134: Service Check Script** ⭐  
**Goal:** Verify service is running  
**Task:** Check if process exists, restart if not  
**Concept:** `pgrep` finds processes  
**Help:** `pgrep nginx || systemctl restart nginx`

**Exercise 135: User Report Script**  
**Goal:** Generate user information  
**Task:** List users with their shell and home  
**Concept:** Parse /etc/passwd  
**Help:** Use awk to extract fields

**Exercise 136: File Cleanup Script**  
**Goal:** Delete old files  
**Task:** Remove files older than 7 days  
**Concept:** `find` with `-mtime`  
**Help:** `find /tmp -mtime +7 -delete`

**Exercise 137: System Info Script** ⭐  
**Goal:** Display system information  
**Task:** Show hostname, IP, disk, memory  
**Concept:** Combine multiple commands  
**Help:** `hostname`, `ip addr`, `df -h`, `free -m`

**Exercise 138: Menu Script**  
**Goal:** Interactive menu system  
**Task:** Display options, read choice, execute  
**Concept:** Combine case with while loop  
**Help:** Use `select` built-in for simple menus

**Exercise 139: Password Generator**  
**Goal:** Create random passwords  
**Task:** Generate random string of specified length  
**Concept:** `/dev/urandom` for randomness  
**Help:** `tr -dc 'A-Za-z0-9' < /dev/urandom | head -c 16`

**Exercise 140: Configuration File Parser** 📝  
**Goal:** Read settings from file  
**Task:** Parse `KEY=VALUE` format  
**Concept:** Source file or parse with grep  
**Help:** `source config.sh` is simplest

---

## 📦 PHASE 3: Package Management & System Administration (Exercises 141-180)

### Week 15: Package Management (Debian/Ubuntu)

**Exercise 141: Update Package Lists** ⭐  
**Goal:** Refresh available packages  
**Task:** `sudo apt update`  
**Concept:** Downloads latest package information  
**Help:** Always run before installing

**Exercise 142: Upgrade All Packages** ⭐  
**Goal:** Update installed packages  
**Task:** `sudo apt upgrade`  
**Concept:** Installs newer versions  
**Help:** `-y` auto-confirms

**Exercise 143: Install a Package** ⭐  
**Goal:** Add new software  
**Task:** `sudo apt install tree`  
**Concept:** `apt install` adds packages  
**Help:** `tree` shows directory structure

**Exercise 144: Remove a Package**  
**Goal:** Uninstall software  
**Task:** `sudo apt remove tree`  
**Concept:** Removes package, keeps config  
**Help:** `purge` removes config too

**Exercise 145: Search for Packages**  
**Goal:** Find available packages  
**Task:** `apt search nginx`  
**Concept:** Search package descriptions  
**Help:** Shows matching packages

**Exercise 146: Show Package Info**  
**Goal:** Get package details  
**Task:** `apt show nginx`  
**Concept:** Shows version, description, dependencies  
**Help:** Useful before installing

**Exercise 147: List Installed Packages**  
**Goal:** See what's installed  
**Task:** `apt list --installed`  
**Concept:** Lists all installed packages  
**Help:** Pipe to grep to filter

**Exercise 148: Clean Package Cache**  
**Goal:** Free up disk space  
**Task:** `sudo apt clean`  
**Concept:** Removes cached package files  
**Help:** Safe to run periodically

**Exercise 149: Autoremove**  
**Goal:** Remove unused dependencies  
**Task:** `sudo apt autoremove`  
**Concept:** Cleans up orphaned packages  
**Help:** Run after removing packages

**Exercise 150: Hold Package Version**  
**Goal:** Prevent package upgrade  
**Task:** `sudo apt-mark hold packagename`  
**Concept:** Keeps package at current version  
**Help:** `unhold` to allow updates again

---

### Week 16: System Services (Systemd)

**Exercise 151: List All Services** ⭐  
**Goal:** See available services  
**Task:** `systemctl list-units --type=service`  
**Concept:** Shows all service units  
**Help:** `--all` includes inactive

**Exercise 152: Check Service Status** ⭐  
**Goal:** See if service is running  
**Task:** `systemctl status nginx`  
**Concept:** Shows running state and recent logs  
**Help:** Green = active, Red = failed

**Exercise 153: Start a Service** ⭐  
**Goal:** Turn on a service  
**Task:** `sudo systemctl start nginx`  
**Concept:** Starts service immediately  
**Help:** Won't survive reboot

**Exercise 154: Stop a Service**  
**Goal:** Turn off a service  
**Task:** `sudo systemctl stop nginx`  
**Concept:** Stops running service  
**Help:** Use for maintenance

**Exercise 155: Restart a Service** ⭐  
**Goal:** Stop and start service  
**Task:** `sudo systemctl restart nginx`  
**Concept:** Applies configuration changes  
**Help:** Brief downtime occurs

**Exercise 156: Reload Configuration**  
**Goal:** Apply changes without restart  
**Task:** `sudo systemctl reload nginx`  
**Concept:** Graceful config reload  
**Help:** No downtime (if supported)

**Exercise 157: Enable at Boot** ⭐  
**Goal:** Start service automatically  
**Task:** `sudo systemctl enable nginx`  
**Concept:** Creates startup symlink  
**Help:** Survives reboots

**Exercise 158: Disable at Boot**  
**Goal:** Stop automatic startup  
**Task:** `sudo systemctl disable nginx`  
**Concept:** Removes startup symlink  
**Help:** Service won't start on boot

**Exercise 159: Enable and Start**  
**Goal:** Do both at once  
**Task:** `sudo systemctl enable --now nginx`  
**Concept:** `--now` also starts immediately  
**Help:** Common combination

**Exercise 160: View Service Logs** ⭐  
**Goal:** See service output  
**Task:** `journalctl -u nginx`  
**Concept:** `journalctl` reads systemd journal  
**Help:** `-f` follows live logs

---

### Week 17: Process & Resource Management

**Exercise 161: Memory Usage**  
**Goal:** Check RAM usage  
**Task:** `free -h`  
**Concept:** Shows total, used, free memory  
**Help:** `-h` = human readable

**Exercise 162: CPU Information**  
**Goal:** See CPU details  
**Task:** `lscpu`  
**Concept:** Shows CPU architecture, cores  
**Help:** Useful for capacity planning

**Exercise 163: Disk Usage Summary** ⭐  
**Goal:** Check disk space  
**Task:** `df -h`  
**Concept:** Shows filesystem usage  
**Help:** Check `/` doesn't fill up!

**Exercise 164: Directory Size**  
**Goal:** Find large directories  
**Task:** `du -sh /var/log`  
**Concept:** `du` = disk usage  
**Help:** `-s` summary, `-h` human readable

**Exercise 165: Find Large Directories** ⭐  
**Goal:** Find what's using space  
**Task:** `du -h --max-depth=1 / | sort -h`  
**Concept:** Sort by size  
**Help:** Helps find disk hogs

**Exercise 166: Process Tree**  
**Goal:** See process hierarchy  
**Task:** `pstree`  
**Concept:** Shows parent-child relationships  
**Help:** `-p` shows PIDs

**Exercise 167: Background Process**  
**Goal:** Run command in background  
**Task:** `command &`  
**Concept:** `&` runs in background  
**Help:** Returns immediately

**Exercise 168: View Background Jobs**  
**Goal:** See background processes  
**Task:** `jobs`  
**Concept:** Lists background jobs  
**Help:** Shows job numbers

**Exercise 169: Bring to Foreground**  
**Goal:** Return to background job  
**Task:** `fg %1`  
**Concept:** `fg` brings job to foreground  
**Help:** `%1` is job number

**Exercise 170: Nohup Command** ⭐  
**Goal:** Run command that survives logout  
**Task:** `nohup long_running_command &`  
**Concept:** Process continues after terminal closes  
**Help:** Output goes to nohup.out

---

### Week 18: Cron Jobs & Scheduling

**Exercise 171: List Cron Jobs**  
**Goal:** See scheduled tasks  
**Task:** `crontab -l`  
**Concept:** Shows your cron entries  
**Help:** Might be empty initially

**Exercise 172: Edit Cron Jobs** ⭐  
**Goal:** Add scheduled tasks  
**Task:** `crontab -e`  
**Concept:** Opens cron editor  
**Help:** Select your preferred editor

**Exercise 173: Cron Format** ⭐ 🎯  
**Goal:** Understand cron timing  
**Task:** Learn `* * * * * command` format  
**Concept:** minute hour day month weekday  
**Help:** `*` means every/any

**Exercise 174: Run Every Minute**  
**Goal:** Test cron works  
**Task:** `* * * * * echo "test" >> /tmp/cron.log`  
**Concept:** Runs every minute  
**Help:** Check /tmp/cron.log

**Exercise 175: Run Hourly**  
**Goal:** Hourly scheduled task  
**Task:** `0 * * * * command`  
**Concept:** Runs at minute 0 of every hour  
**Help:** At :00 of every hour

**Exercise 176: Run Daily** ⭐  
**Goal:** Once per day  
**Task:** `0 2 * * * command`  
**Concept:** Runs at 2:00 AM daily  
**Help:** Good for backups

**Exercise 177: Run Weekly**  
**Goal:** Once per week  
**Task:** `0 2 * * 0 command`  
**Concept:** Sunday at 2:00 AM  
**Help:** 0 = Sunday, 1 = Monday...

**Exercise 178: Run Monthly**  
**Goal:** Once per month  
**Task:** `0 2 1 * * command`  
**Concept:** 1st day of month at 2:00 AM  
**Help:** Good for monthly reports

**Exercise 179: Every 5 Minutes**  
**Goal:** Frequent checking  
**Task:** `*/5 * * * * command`  
**Concept:** `*/5` = every 5  
**Help:** Common for monitoring

**Exercise 180: Cron with Logging** 📝  
**Goal:** Capture cron output  
**Task:** `* * * * * command >> /var/log/myjob.log 2>&1`  
**Concept:** Redirect output and errors  
**Help:** Essential for debugging

---

## 🌐 PHASE 4: Networking Fundamentals (Exercises 181-230)

### Week 19: Network Basics

**Exercise 181: View IP Address** ⭐  
**Goal:** Find your IP address  
**Task:** `ip addr show`  
**Concept:** Shows network interface info  
**Help:** Look for `inet` line

**Exercise 182: Shorter IP Command**  
**Goal:** Quicker IP viewing  
**Task:** `ip a`  
**Concept:** `a` is shorthand for `addr`  
**Help:** Common abbreviation

**Exercise 183: View Only IPv4**  
**Goal:** Filter to IPv4  
**Task:** `ip -4 addr`  
**Concept:** `-4` filters to IPv4 only  
**Help:** `-6` for IPv6

**Exercise 184: Hostname** ⭐  
**Goal:** View/set hostname  
**Task:** `hostname`  
**Concept:** System's network name  
**Help:** `hostnamectl` for more info

**Exercise 185: Change Hostname**  
**Goal:** Set new hostname  
**Task:** `sudo hostnamectl set-hostname newname`  
**Concept:** Persistent hostname change  
**Help:** May need to update /etc/hosts

**Exercise 186: View Routing Table**  
**Goal:** See network routes  
**Task:** `ip route` or `route -n`  
**Concept:** Shows how traffic is directed  
**Help:** Default route is your gateway

**Exercise 187: DNS Resolution** ⭐  
**Goal:** Look up domain to IP  
**Task:** `nslookup google.com`  
**Concept:** DNS translates names to IPs  
**Help:** `dig` gives more detail

**Exercise 188: View DNS Config**  
**Goal:** See DNS servers  
**Task:** `cat /etc/resolv.conf`  
**Concept:** System DNS configuration  
**Help:** `nameserver` entries

**Exercise 189: Hosts File** ⭐  
**Goal:** Local name resolution  
**Task:** `cat /etc/hosts`  
**Concept:** Local DNS override  
**Help:** Checked before DNS

**Exercise 190: Add Hosts Entry**  
**Goal:** Create local DNS entry  
**Task:** Add `192.168.1.100 myserver` to /etc/hosts  
**Concept:** Custom name resolution  
**Help:** Useful for local development

---

### Week 20: Network Testing

**Exercise 191: Ping Test** ⭐  
**Goal:** Test network connectivity  
**Task:** `ping -c 4 google.com`  
**Concept:** Sends ICMP echo requests  
**Help:** `-c 4` sends 4 pings

**Exercise 192: Ping Local Network**  
**Goal:** Test local connectivity  
**Task:** Ping your gateway IP  
**Concept:** Verify network is working  
**Help:** Gateway IP from `ip route`

**Exercise 193: Traceroute**  
**Goal:** See network path  
**Task:** `traceroute google.com`  
**Concept:** Shows hops to destination  
**Help:** `tracepath` is alternative

**Exercise 194: Check Open Ports** ⭐  
**Goal:** See listening services  
**Task:** `ss -tlnp`  
**Concept:** Shows TCP listening ports  
**Help:** `-t` TCP, `-l` listening, `-n` numeric, `-p` process

**Exercise 195: Netstat Alternative**  
**Goal:** Old way to see ports  
**Task:** `netstat -tlnp`  
**Concept:** Similar to ss  
**Help:** `ss` is newer and faster

**Exercise 196: Test Port Connection** ⭐  
**Goal:** Check if port is open  
**Task:** `nc -zv localhost 22`  
**Concept:** Netcat tests connectivity  
**Help:** `-z` scan only, `-v` verbose

**Exercise 197: Download File** ⭐  
**Goal:** Get file from web  
**Task:** `curl -O https://example.com/file`  
**Concept:** `curl` transfers data  
**Help:** `-O` saves with original name

**Exercise 198: Wget Download**  
**Goal:** Alternative download tool  
**Task:** `wget https://example.com/file`  
**Concept:** `wget` retrieves files  
**Help:** Simpler for basic downloads

**Exercise 199: View HTTP Headers**  
**Goal:** See response headers  
**Task:** `curl -I https://example.com`  
**Concept:** `-I` shows headers only  
**Help:** Good for debugging

**Exercise 200: Test API** ⭐  
**Goal:** Make HTTP request  
**Task:** `curl https://api.github.com`  
**Concept:** curl for API testing  
**Help:** Returns JSON response

---

### Week 21: Firewall Basics (UFW)

**Exercise 201: Check Firewall Status**  
**Goal:** See if firewall active  
**Task:** `sudo ufw status`  
**Concept:** UFW = Uncomplicated Firewall  
**Help:** Shows active/inactive

**Exercise 202: Enable Firewall** ⭐ ⚠️  
**Goal:** Turn on firewall  
**Task:** `sudo ufw enable`  
**Concept:** Starts blocking traffic  
**Warning:** Make sure SSH is allowed first!

**Exercise 203: Allow SSH First!** ⭐  
**Goal:** Don't lock yourself out  
**Task:** `sudo ufw allow ssh` or `sudo ufw allow 22`  
**Concept:** SSH access is critical  
**Help:** Always do this before enabling!

**Exercise 204: Allow HTTP**  
**Goal:** Allow web traffic  
**Task:** `sudo ufw allow 80`  
**Concept:** Opens port 80  
**Help:** For web servers

**Exercise 205: Allow HTTPS**  
**Goal:** Allow secure web traffic  
**Task:** `sudo ufw allow 443`  
**Concept:** Opens port 443  
**Help:** For HTTPS

**Exercise 206: Allow Specific Port**  
**Goal:** Open custom port  
**Task:** `sudo ufw allow 8080`  
**Concept:** Opens any port you specify  
**Help:** For custom applications

**Exercise 207: Deny a Port**  
**Goal:** Block specific port  
**Task:** `sudo ufw deny 23`  
**Concept:** Explicitly blocks port  
**Help:** 23 is Telnet (insecure)

**Exercise 208: Allow from IP**  
**Goal:** Allow specific source  
**Task:** `sudo ufw allow from 192.168.1.100`  
**Concept:** Source-based filtering  
**Help:** Only that IP can connect

**Exercise 209: Delete Rule**  
**Goal:** Remove firewall rule  
**Task:** `sudo ufw delete allow 8080`  
**Concept:** Removes specific rule  
**Help:** Or use rule number

**Exercise 210: View Numbered Rules**  
**Goal:** See rules with numbers  
**Task:** `sudo ufw status numbered`  
**Concept:** Numbers make deletion easier  
**Help:** `sudo ufw delete 3` removes rule 3

---

### Week 22: SSH & Remote Access

**Exercise 211: Connect via SSH** ⭐  
**Goal:** Log into remote server  
**Task:** `ssh user@hostname`  
**Concept:** Secure Shell connection  
**Help:** Replace with actual user/host

**Exercise 212: SSH with Port**  
**Goal:** Connect to non-default port  
**Task:** `ssh -p 2222 user@hostname`  
**Concept:** `-p` specifies port  
**Help:** Default is 22

**Exercise 213: Generate SSH Key** ⭐  
**Goal:** Create key pair  
**Task:** `ssh-keygen -t ed25519`  
**Concept:** Public/private key authentication  
**Help:** Accept defaults, set passphrase

**Exercise 214: View Public Key**  
**Goal:** See your public key  
**Task:** `cat ~/.ssh/id_ed25519.pub`  
**Concept:** This is safe to share  
**Help:** Copy this to remote servers

**Exercise 215: Copy Key to Server** ⭐  
**Goal:** Enable key-based login  
**Task:** `ssh-copy-id user@hostname`  
**Concept:** Installs key on remote  
**Help:** Then no password needed

**Exercise 216: SSH Config File**  
**Goal:** Create shortcuts  
**Task:** Edit `~/.ssh/config`  
**Concept:** Save connection settings  
**Help:** `Host myserver`

**Exercise 217: Simple SSH Config**  
**Goal:** Configure a host  
**Task:** Add Host, HostName, User, Port  
**Concept:** Then just `ssh myserver`  
**Help:** Much easier than full command

**Exercise 218: SCP File Transfer** ⭐  
**Goal:** Copy file to remote  
**Task:** `scp file.txt user@host:/path/`  
**Concept:** Secure Copy Protocol  
**Help:** Works like `cp` but remote

**Exercise 219: SCP Directory**  
**Goal:** Copy folder to remote  
**Task:** `scp -r folder/ user@host:/path/`  
**Concept:** `-r` for recursive  
**Help:** Copies entire directory

**Exercise 220: Rsync Basics** ⭐  
**Goal:** Sync files efficiently  
**Task:** `rsync -avz source/ user@host:/dest/`  
**Concept:** Only transfers changes  
**Help:** `-a` archive, `-v` verbose, `-z` compress

---

### Week 23: Network Services

**Exercise 221: HTTP Server Quick Start**  
**Goal:** Serve files locally  
**Task:** `python3 -m http.server 8000`  
**Concept:** Instant web server  
**Help:** Access at localhost:8000

**Exercise 222: Check Who's Listening**  
**Goal:** See all listening ports  
**Task:** `ss -tuln`  
**Concept:** TCP and UDP listeners  
**Help:** `-u` adds UDP

**Exercise 223: View Active Connections**  
**Goal:** See established connections  
**Task:** `ss -tn`  
**Concept:** Shows connected sessions  
**Help:** Without `-l` shows established

**Exercise 224: Network Interface Stats**  
**Goal:** See traffic statistics  
**Task:** `ip -s link`  
**Concept:** Shows bytes/packets  
**Help:** `-s` adds statistics

**Exercise 225: ARP Table**  
**Goal:** See local network devices  
**Task:** `ip neigh` or `arp -a`  
**Concept:** Maps IPs to MAC addresses  
**Help:** Shows local network devices

**Exercise 226: TCP Dump Basics** ⚠️  
**Goal:** Capture network traffic  
**Task:** `sudo tcpdump -i any -c 10`  
**Concept:** Packet capture  
**Help:** `-c 10` captures 10 packets

**Exercise 227: Filter TCP Dump**  
**Goal:** Capture specific traffic  
**Task:** `sudo tcpdump port 80`  
**Concept:** Filter by port  
**Help:** Only HTTP traffic

**Exercise 228: Save Capture**  
**Goal:** Save for analysis  
**Task:** `sudo tcpdump -w capture.pcap`  
**Concept:** Write to file  
**Help:** Open with Wireshark

**Exercise 229: Network Namespace Intro**  
**Goal:** Understand isolation  
**Task:** `ip netns list`  
**Concept:** Isolated network stacks  
**Help:** Used by containers

**Exercise 230: MTU Check**  
**Goal:** View Maximum Transmission Unit  
**Task:** `ip link show eth0`  
**Concept:** MTU affects packet size  
**Help:** Default is usually 1500

---

## 🐳 PHASE 5: Docker Fundamentals (Exercises 231-310)

### Week 24: Docker Basics

**Exercise 231: Install Docker** ⭐  
**Goal:** Get Docker running  
**Task:** Follow Docker's official install guide for your distro  
**Concept:** Container runtime  
**Help:** `curl -fsSL https://get.docker.com | sh`

**Exercise 232: Verify Installation**  
**Goal:** Confirm Docker works  
**Task:** `docker --version`  
**Concept:** Check version installed  
**Help:** Should show version number

**Exercise 233: Run Without Sudo**  
**Goal:** Add user to docker group  
**Task:** `sudo usermod -aG docker $USER`  
**Concept:** Avoid typing sudo  
**Help:** Log out and back in

**Exercise 234: Hello World Container** ⭐  
**Goal:** Run first container  
**Task:** `docker run hello-world`  
**Concept:** Pulls and runs image  
**Help:** Tests Docker installation

**Exercise 235: Run Ubuntu Container** ⭐  
**Goal:** Interactive container  
**Task:** `docker run -it ubuntu bash`  
**Concept:** `-it` = interactive + terminal  
**Help:** You're now inside Ubuntu!

**Exercise 236: Exit Container**  
**Goal:** Leave container  
**Task:** Type `exit` or press `Ctrl+D`  
**Concept:** Stops container when you exit  
**Help:** Container stops too

**Exercise 237: List Running Containers** ⭐  
**Goal:** See active containers  
**Task:** `docker ps`  
**Concept:** Shows running containers  
**Help:** Like `ps` for containers

**Exercise 238: List All Containers**  
**Goal:** Include stopped containers  
**Task:** `docker ps -a`  
**Concept:** Shows all containers ever run  
**Help:** `-a` = all

**Exercise 239: Run in Background** ⭐  
**Goal:** Detached container  
**Task:** `docker run -d nginx`  
**Concept:** `-d` = detached mode  
**Help:** Returns container ID

**Exercise 240: Container Logs** ⭐  
**Goal:** View container output  
**Task:** `docker logs container_id`  
**Concept:** Shows stdout/stderr  
**Help:** `-f` follows live

---

### Week 25: Container Management

**Exercise 241: Stop Container** ⭐  
**Goal:** Gracefully stop container  
**Task:** `docker stop container_id`  
**Concept:** Sends SIGTERM then SIGKILL  
**Help:** 10 second grace period

**Exercise 242: Start Container**  
**Goal:** Start stopped container  
**Task:** `docker start container_id`  
**Concept:** Starts existing container  
**Help:** Keeps previous config

**Exercise 243: Restart Container**  
**Goal:** Stop and start  
**Task:** `docker restart container_id`  
**Concept:** Quick restart  
**Help:** Useful after config changes

**Exercise 244: Remove Container** ⭐  
**Goal:** Delete stopped container  
**Task:** `docker rm container_id`  
**Concept:** Cleans up container  
**Help:** Must be stopped first

**Exercise 245: Force Remove**  
**Goal:** Delete running container  
**Task:** `docker rm -f container_id`  
**Concept:** `-f` forces removal  
**Help:** Stops then removes

**Exercise 246: Remove All Stopped**  
**Goal:** Clean up old containers  
**Task:** `docker container prune`  
**Concept:** Removes all stopped  
**Help:** Confirms before deleting

**Exercise 247: Name Your Container** ⭐  
**Goal:** Give container a name  
**Task:** `docker run --name myapp -d nginx`  
**Concept:** Named containers are easier to manage  
**Help:** Use instead of container ID

**Exercise 248: Execute in Container** ⭐  
**Goal:** Run command inside container  
**Task:** `docker exec -it myapp bash`  
**Concept:** `exec` runs in running container  
**Help:** Great for debugging

**Exercise 249: Inspect Container**  
**Goal:** See container details  
**Task:** `docker inspect container_id`  
**Concept:** JSON with all config  
**Help:** Lots of detail!

**Exercise 250: Container Stats**  
**Goal:** Monitor resource usage  
**Task:** `docker stats`  
**Concept:** Live CPU/memory usage  
**Help:** Press `Ctrl+C` to exit

---

### Week 26: Docker Images

**Exercise 251: List Images** ⭐  
**Goal:** See local images  
**Task:** `docker images`  
**Concept:** Images stored locally  
**Help:** Shows size and tags

**Exercise 252: Pull an Image** ⭐  
**Goal:** Download image from registry  
**Task:** `

`docker pull nginx`  
**Concept:** Downloads from Docker Hub  
**Help:** Without run, just downloads

**Exercise 253: Pull Specific Version**  
**Goal:** Get specific image tag  
**Task:** `docker pull nginx:1.24`  
**Concept:** Tags specify versions  
**Help:** `:latest` is default

**Exercise 254: Search Images**  
**Goal:** Find images on Docker Hub  
**Task:** `docker search python`  
**Concept:** Search registry  
**Help:** Shows official and community

**Exercise 255: Remove Image** ⭐  
**Goal:** Delete local image  
**Task:** `docker rmi nginx`  
**Concept:** Remove image  
**Help:** Container must not be using it

**Exercise 256: Remove Unused Images**  
**Goal:** Clean up disk space  
**Task:** `docker image prune`  
**Concept:** Removes dangling images  
**Help:** `-a` removes all unused

**Exercise 257: Image History**  
**Goal:** See image layers  
**Task:** `docker history nginx`  
**Concept:** Shows build steps  
**Help:** Each layer adds to image

**Exercise 258: Tag an Image**  
**Goal:** Add custom tag  
**Task:** `docker tag nginx myregistry/nginx:v1`  
**Concept:** Tags for versioning  
**Help:** Needed for pushing

**Exercise 259: Save Image to File**  
**Goal:** Export image  
**Task:** `docker save nginx > nginx.tar`  
**Concept:** Archive image  
**Help:** For offline transfer

**Exercise 260: Load Image from File**  
**Goal:** Import saved image  
**Task:** `docker load < nginx.tar`  
**Concept:** Restore archived image  
**Help:** Works offline

---

### Week 27: Building Docker Images

**Exercise 261: Create Dockerfile** ⭐  
**Goal:** Write first Dockerfile  
**Task:** Create file named `Dockerfile` with `FROM ubuntu`  
**Concept:** Dockerfile defines image  
**Help:** Just one line to start

**Exercise 262: Build Image** ⭐  
**Goal:** Create image from Dockerfile  
**Task:** `docker build -t myimage .`  
**Concept:** `-t` tags the image  
**Help:** `.` is build context

**Exercise 263: FROM Instruction** ⭐  
**Goal:** Set base image  
**Task:** `FROM python:3.11`  
**Concept:** Every Dockerfile starts with FROM  
**Help:** Start from existing image

**Exercise 264: RUN Instruction** ⭐  
**Goal:** Execute commands during build  
**Task:** `RUN apt-get update && apt-get install -y curl`  
**Concept:** RUN creates new layer  
**Help:** Combine with && to reduce layers

**Exercise 265: COPY Instruction** ⭐  
**Goal:** Add files to image  
**Task:** `COPY app.py /app/`  
**Concept:** Copies from host to image  
**Help:** Source then destination

**Exercise 266: WORKDIR Instruction**  
**Goal:** Set working directory  
**Task:** `WORKDIR /app`  
**Concept:** Like `cd` for container  
**Help:** Creates dir if needed

**Exercise 267: CMD Instruction** ⭐  
**Goal:** Default command  
**Task:** `CMD ["python", "app.py"]`  
**Concept:** Runs when container starts  
**Help:** Can be overridden

**Exercise 268: ENTRYPOINT Instruction**  
**Goal:** Fixed command  
**Task:** `ENTRYPOINT ["python"]`  
**Concept:** Cannot be easily overridden  
**Help:** CMD becomes arguments

**Exercise 269: EXPOSE Instruction**  
**Goal:** Document ports  
**Task:** `EXPOSE 8080`  
**Concept:** Documents which ports  
**Help:** Doesn't actually publish!

**Exercise 270: ENV Instruction** ⭐  
**Goal:** Set environment variables  
**Task:** `ENV APP_ENV=production`  
**Concept:** Available at runtime  
**Help:** Can be overridden with -e

---

### Week 28: Docker Networking

**Exercise 271: List Networks**  
**Goal:** See Docker networks  
**Task:** `docker network ls`  
**Concept:** Docker has network drivers  
**Help:** bridge, host, none

**Exercise 272: Inspect Bridge Network**  
**Goal:** View default network  
**Task:** `docker network inspect bridge`  
**Concept:** Default container network  
**Help:** Shows connected containers

**Exercise 273: Create Network** ⭐  
**Goal:** Create custom network  
**Task:** `docker network create mynetwork`  
**Concept:** Custom networks for apps  
**Help:** Better than default bridge

**Exercise 274: Connect Container to Network**  
**Goal:** Join network at runtime  
**Task:** `docker run --network mynetwork -d nginx`  
**Concept:** Containers can communicate  
**Help:** Use container names as DNS

**Exercise 275: Container DNS** ⭐  
**Goal:** Containers resolve by name  
**Task:** Ping one container from another by name  
**Concept:** Automatic DNS in custom networks  
**Help:** Only in custom networks!

**Exercise 276: Publish Port** ⭐  
**Goal:** Make container accessible  
**Task:** `docker run -p 8080:80 nginx`  
**Concept:** Map host port to container  
**Help:** `-p hostPort:containerPort`

**Exercise 277: Publish All Ports**  
**Goal:** Random host ports  
**Task:** `docker run -P nginx`  
**Concept:** Maps all EXPOSE ports  
**Help:** Use `docker ps` to see ports

**Exercise 278: Host Network Mode**  
**Goal:** Use host networking  
**Task:** `docker run --network host nginx`  
**Concept:** Container uses host network  
**Help:** No port mapping needed

**Exercise 279: Link Containers (Legacy)**  
**Goal:** Understand legacy linking  
**Task:** `docker run --link db:database web`  
**Concept:** Old way to connect  
**Help:** Use networks instead!

**Exercise 280: Remove Network**  
**Goal:** Delete custom network  
**Task:** `docker network rm mynetwork`  
**Concept:** Clean up unused networks  
**Help:** Disconnect containers first

---

### Week 29: Docker Volumes

**Exercise 281: Create Named Volume** ⭐  
**Goal:** Persistent storage  
**Task:** `docker volume create mydata`  
**Concept:** Data survives container  
**Help:** Stored on host

**Exercise 282: List Volumes**  
**Goal:** See all volumes  
**Task:** `docker volume ls`  
**Concept:** Shows volume names  
**Help:** Named and anonymous

**Exercise 283: Use Volume** ⭐  
**Goal:** Mount volume to container  
**Task:** `docker run -v mydata:/app/data nginx`  
**Concept:** `-v name:/path`  
**Help:** Data persists after container removed

**Exercise 284: Bind Mount** ⭐  
**Goal:** Mount host directory  
**Task:** `docker run -v /host/path:/container/path nginx`  
**Concept:** Direct host access  
**Help:** Use absolute paths

**Exercise 285: Read-Only Mount**  
**Goal:** Protect host data  
**Task:** `docker run -v /data:/data:ro nginx`  
**Concept:** `:ro` makes read-only  
**Help:** Container can't modify

**Exercise 286: Inspect Volume**  
**Goal:** View volume details  
**Task:** `docker volume inspect mydata`  
**Concept:** Shows mount point  
**Help:** See where data lives

**Exercise 287: Remove Volume**  
**Goal:** Delete volume  
**Task:** `docker volume rm mydata`  
**Concept:** Permanent deletion!  
**Help:** Make sure data isn't needed

**Exercise 288: Prune Volumes**  
**Goal:** Clean unused volumes  
**Task:** `docker volume prune`  
**Concept:** Removes unused volumes  
**Help:** Frees disk space

**Exercise 289: Volume in Dockerfile**  
**Goal:** Declare volume in image  
**Task:** `VOLUME /app/data`  
**Concept:** Creates mount point  
**Help:** Anonymous volume created

**Exercise 290: Backup Volume** 📝  
**Goal:** Export volume data  
**Task:** Use container to tar volume contents  
**Concept:** Volumes need backup strategy  
**Help:** `docker run --rm -v mydata:/data -v $(pwd):/backup alpine tar cvf /backup/backup.tar /data`

---

### Week 30: Docker Compose Basics

**Exercise 291: Install Docker Compose** ⭐  
**Goal:** Get compose running  
**Task:** Usually included with Docker Desktop, or install separately  
**Concept:** Multi-container tool  
**Help:** `docker compose version`

**Exercise 292: Create compose.yaml** ⭐  
**Goal:** Write first compose file  
**Task:** Create `compose.yaml` with version and services  
**Concept:** YAML defines application  
**Help:** Previously called docker-compose.yml

**Exercise 293: Simple Compose File**  
**Goal:** Define single service  
**Task:** Define web service with nginx image  
**Concept:** Services are containers  
**Help:** `services:` then `web:` then `image: nginx`

**Exercise 294: Docker Compose Up** ⭐  
**Goal:** Start application  
**Task:** `docker compose up`  
**Concept:** Creates and starts all services  
**Help:** `-d` for detached

**Exercise 295: Docker Compose Down** ⭐  
**Goal:** Stop and remove  
**Task:** `docker compose down`  
**Concept:** Stops and removes containers  
**Help:** Networks removed too

**Exercise 296: View Compose Logs**  
**Goal:** See all service logs  
**Task:** `docker compose logs`  
**Concept:** Aggregated logs  
**Help:** `-f` follows

**Exercise 297: Multiple Services** ⭐  
**Goal:** Define web + db  
**Task:** Add postgres service to compose  
**Concept:** Services can communicate  
**Help:** Use service name as hostname

**Exercise 298: Compose Ports**  
**Goal:** Publish ports  
**Task:** `ports: - "8080:80"`  
**Concept:** Same as -p flag  
**Help:** List of port mappings

**Exercise 299: Compose Volumes**  
**Goal:** Add volumes  
**Task:** `volumes: - mydata:/var/lib/data`  
**Concept:** Named volumes in compose  
**Help:** Define at service and top level

**Exercise 300: Compose Environment**  
**Goal:** Set environment variables  
**Task:** `environment: - DB_HOST=postgres`  
**Concept:** Configure services  
**Help:** Or use env_file

---

### Week 31: Advanced Docker Compose

**Exercise 301: Build in Compose** ⭐  
**Goal:** Build from Dockerfile  
**Task:** `build: ./app` instead of image  
**Concept:** Compose can build  
**Help:** Point to directory with Dockerfile

**Exercise 302: Depends On**  
**Goal:** Set service order  
**Task:** `depends_on: - db`  
**Concept:** Start order dependency  
**Help:** Doesn't wait for ready!

**Exercise 303: Health Checks**  
**Goal:** Define service health  
**Task:** Add healthcheck to service  
**Concept:** Docker monitors health  
**Help:** `test`, `interval`, `timeout`

**Exercise 304: Restart Policy**  
**Goal:** Auto restart containers  
**Task:** `restart: unless-stopped`  
**Concept:** Handles crashes  
**Help:** `always`, `on-failure`, `unless-stopped`

**Exercise 305: Resource Limits**  
**Goal:** Limit CPU and memory  
**Task:** Add `deploy: resources: limits:`  
**Concept:** Prevent resource hogging  
**Help:** `cpus: '0.5'` and `memory: 512M`

**Exercise 306: Compose Profiles**  
**Goal:** Optional services  
**Task:** `profiles: - debug`  
**Concept:** Enable services selectively  
**Help:** `docker compose --profile debug up`

**Exercise 307: Environment Files**  
**Goal:** Load env from file  
**Task:** `env_file: - .env`  
**Concept:** Separate config from compose  
**Help:** `.env` file with KEY=VALUE

**Exercise 308: Compose Override**  
**Goal:** Environment-specific config  
**Task:** Create `compose.override.yaml`  
**Concept:** Overrides merged automatically  
**Help:** For dev-specific settings

**Exercise 309: Compose Scale**  
**Goal:** Run multiple instances  
**Task:** `docker compose up --scale web=3`  
**Concept:** Horizontal scaling  
**Help:** Load balancer needed

**Exercise 310: Complete App Stack** 📝 🎯  
**Goal:** Full application  
**Task:** Compose with frontend, backend, database, volumes  
**Concept:** Real-world application  
**Help:** Practice complete setups

---

## 📊 PHASE 6: Monitoring & Logging (Exercises 311-360)

### Week 32: System Monitoring

**Exercise 311: Uptime Command**  
**Goal:** Check system uptime  
**Task:** `uptime`  
**Concept:** Shows how long system running  
**Help:** Also shows load averages

**Exercise 312: Load Average** ⭐  
**Goal:** Understand system load  
**Task:** Interpret load from `uptime`  
**Concept:** 1, 5, 15 minute averages  
**Help:** Divide by CPU count

**Exercise 313: Vmstat Command**  
**Goal:** Virtual memory statistics  
**Task:** `vmstat 1 5`  
**Concept:** Memory, swap, I/O, CPU  
**Help:** 1 second interval, 5 times

**Exercise 314: Iostat Command**  
**Goal:** Disk I/O statistics  
**Task:** `iostat -x 1`  
**Concept:** Disk read/write stats  
**Help:** `-x` extended statistics

**Exercise 315: Iotop Command**  
**Goal:** Disk I/O by process  
**Task:** `sudo iotop`  
**Concept:** Which process uses disk  
**Help:** Like top for I/O

**Exercise 316: Sar Command**  
**Goal:** Historical statistics  
**Task:** `sar -u 1 5`  
**Concept:** CPU utilization over time  
**Help:** Part of sysstat package

**Exercise 317: Watch Command** ⭐  
**Goal:** Repeat command  
**Task:** `watch -n 2 'df -h'`  
**Concept:** Updates every 2 seconds  
**Help:** Monitor changes

**Exercise 318: Dmesg Command**  
**Goal:** Kernel messages  
**Task:** `dmesg | tail -20`  
**Concept:** Hardware and kernel events  
**Help:** `-T` for timestamps

**Exercise 319: System Journal** ⭐  
**Goal:** View system logs  
**Task:** `journalctl`  
**Concept:** Centralized logging  
**Help:** `-e` jumps to end

**Exercise 320: Journal for Service**  
**Goal:** Logs for specific service  
**Task:** `journalctl -u nginx`  
**Concept:** Filter by unit  
**Help:** `-f` follows live

---

### Week 33: Log Management

**Exercise 321: View Syslog**  
**Goal:** System messages  
**Task:** `tail -f /var/log/syslog`  
**Concept:** Central system log  
**Help:** Or /var/log/messages

**Exercise 322: Auth Log**  
**Goal:** Security events  
**Task:** `sudo tail /var/log/auth.log`  
**Concept:** Login attempts  
**Help:** Watch for failed logins

**Exercise 323: Boot Log**  
**Goal:** Startup messages  
**Task:** `journalctl -b`  
**Concept:** Current boot logs  
**Help:** `-b -1` for previous boot

**Exercise 324: Log Priority Filter**  
**Goal:** Filter by severity  
**Task:** `journalctl -p err`  
**Concept:** Priorities: emerg, alert, crit, err, warning, notice, info, debug  
**Help:** Shows selected and higher

**Exercise 325: Time-Based Logs**  
**Goal:** Logs from time period  
**Task:** `journalctl --since "1 hour ago"`  
**Concept:** Filter by time  
**Help:** `--until` for end time

**Exercise 326: Log Disk Usage**  
**Goal:** Check log sizes  
**Task:** `du -sh /var/log/*`  
**Concept:** Logs can fill disk  
**Help:** Monitor regularly

**Exercise 327: Logrotate Config**  
**Goal:** Understand log rotation  
**Task:** `cat /etc/logrotate.conf`  
**Concept:** Automatic log management  
**Help:** Compresses old logs

**Exercise 328: Custom Logrotate**  
**Goal:** Configure app log rotation  
**Task:** Create `/etc/logrotate.d/myapp`  
**Concept:** Per-app rotation settings  
**Help:** Size, count, compression

**Exercise 329: Logger Command**  
**Goal:** Write to syslog  
**Task:** `logger "My custom message"`  
**Concept:** Send messages to log  
**Help:** Useful in scripts

**Exercise 330: Grep Logs** ⭐ 🎯  
**Goal:** Search log files  
**Task:** `grep -i error /var/log/syslog`  
**Concept:** Filter for patterns  
**Help:** `-i` case insensitive

---

### Week 34: Prometheus Basics

**Exercise 331: Install Prometheus** ⭐  
**Goal:** Set up monitoring  
**Task:** Download and run Prometheus  
**Concept:** Time-series database  
**Help:** Run locally with docker

**Exercise 332: Prometheus Config**  
**Goal:** Understand prometheus.yml  
**Task:** View default configuration  
**Concept:** Defines scrape targets  
**Help:** Targets are things to monitor

**Exercise 333: Access Prometheus UI**  
**Goal:** Open web interface  
**Task:** Go to http://localhost:9090  
**Concept:** Query and explore metrics  
**Help:** Default port is 9090

**Exercise 334: Basic PromQL** ⭐  
**Goal:** Query metrics  
**Task:** Query `up` metric  
**Concept:** PromQL is query language  
**Help:** Shows target status

**Exercise 335: Node Exporter**  
**Goal:** Collect host metrics  
**Task:** Run node_exporter  
**Concept:** Exposes system metrics  
**Help:** CPU, memory, disk, network

**Exercise 336: Add Scrape Target**  
**Goal:** Monitor node_exporter  
**Task:** Add target to prometheus.yml  
**Concept:** Prometheus pulls metrics  
**Help:** Restart after config change

**Exercise 337: Filter by Label**  
**Goal:** Select specific metrics  
**Task:** `node_cpu_seconds_total{mode="idle"}`  
**Concept:** Labels filter data  
**Help:** Curly braces for labels

**Exercise 338: Rate Function** ⭐  
**Goal:** Calculate rate of change  
**Task:** `rate(node_cpu_seconds_total[5m])`  
**Concept:** Per-second rate over time  
**Help:** Essential for counters

**Exercise 339: Aggregation**  
**Goal:** Sum across instances  
**Task:** `sum(rate(node_cpu_seconds_total[5m]))`  
**Concept:** Aggregate functions  
**Help:** sum, avg, max, min, count

**Exercise 340: Recording Rules**  
**Goal:** Pre-compute queries  
**Task:** Create rule file  
**Concept:** Save expensive queries  
**Help:** Faster dashboards

---

### Week 35: Grafana Basics

**Exercise 341: Install Grafana** ⭐  
**Goal:** Set up dashboards  
**Task:** Run Grafana with Docker  
**Concept:** Visualization platform  
**Help:** Default port 3000

**Exercise 342: First Login**  
**Goal:** Access Grafana  
**Task:** Login with admin/admin  
**Concept:** Default credentials  
**Help:** Change password immediately!

**Exercise 343: Add Prometheus Data Source** ⭐  
**Goal:** Connect to Prometheus  
**Task:** Configuration → Data Sources → Add  
**Concept:** Grafana queries data sources  
**Help:** URL is Prometheus address

**Exercise 344: Create Dashboard** ⭐  
**Goal:** New dashboard  
**Task:** Create → Dashboard  
**Concept:** Dashboards contain panels  
**Help:** Start empty

**Exercise 345: Add Panel**  
**Goal:** Create visualization  
**Task:** Add new panel  
**Concept:** Panels show metrics  
**Help:** Choose visualization type

**Exercise 346: Query in Panel**  
**Goal:** Display metric  
**Task:** Enter PromQL query  
**Concept:** Each panel has queries  
**Help:** Same syntax as Prometheus

**Exercise 347: Panel Options**  
**Goal:** Customize display  
**Task:** Set title, description, units  
**Concept:** Make panels readable  
**Help:** Units help interpretation

**Exercise 348: Time Range**  
**Goal:** Adjust time window  
**Task:** Use time picker  
**Concept:** View different periods  
**Help:** Last 5m, 1h, 24h, etc.

**Exercise 349: Import Dashboard**  
**Goal:** Use pre-built dashboard  
**Task:** Import node exporter dashboard  
**Concept:** Community dashboards  
**Help:** Dashboard ID: 1860

**Exercise 350: Dashboard Variables**  
**Goal:** Dynamic filtering  
**Task:** Add variable to dashboard  
**Concept:** Drop-down filters  
**Help:** Filter by host, service, etc.

---

### Week 36: Alerting

**Exercise 351: Grafana Alerts** ⭐  
**Goal:** Create alert rule  
**Task:** Add alert to panel  
**Concept:** Notify on conditions  
**Help:** Alerting → Alert rules

**Exercise 352: Alert Conditions**  
**Goal:** Define when to alert  
**Task:** Set threshold condition  
**Concept:** IS ABOVE, IS BELOW, etc.  
**Help:** Test with current values

**Exercise 353: Notification Channel**  
**Goal:** Where to send alerts  
**Task:** Create notification channel  
**Concept:** Email, Slack, webhook  
**Help:** Alerting → Notification channels

**Exercise 354: Prometheus Alerting**  
**Goal:** Alerts in Prometheus  
**Task:** Create alerting rules  
**Concept:** Prometheus can alert  
**Help:** rules.yml file

**Exercise 355: Alertmanager**  
**Goal:** Route alerts  
**Task:** Run Alertmanager  
**Concept:** Handles alert routing  
**Help:** Deduplication, grouping

**Exercise 356: Alert Severity**  
**Goal:** Priority levels  
**Task:** Add severity label  
**Concept:** critical, warning, info  
**Help:** Route based on severity

**Exercise 357: Silence Alerts**  
**Goal:** Temporarily mute  
**Task:** Create silence in Alertmanager  
**Concept:** Maintenance windows  
**Help:** Set start and end time

**Exercise 358: Alert Testing**  
**Goal:** Verify alerts work  
**Task:** Trigger test alert  
**Concept:** Always test alerting  
**Help:** Lower threshold temporarily

**Exercise 359: Runbook Links**  
**Goal:** Link to documentation  
**Task:** Add runbook_url annotation  
**Concept:** Help responders  
**Help:** Points to fix procedure

**Exercise 360: On-Call Rotation** 📝  
**Goal:** Understand on-call  
**Task:** Design alert response process  
**Concept:** Who responds to alerts  
**Help:** Document escalation path

---

## 🔄 PHASE 7: Version Control with Git (Exercises 361-420)

### Week 37: Git Basics

**Exercise 361: Install Git** ⭐  
**Goal:** Get Git installed  
**Task:** `sudo apt install git`  
**Concept:** Distributed version control  
**Help:** `git --version` to verify

**Exercise 362: Configure Name** ⭐  
**Goal:** Set your identity  
**Task:** `git config --global user.name "Your Name"`  
**Concept:** Commits need author  
**Help:** Use your real name

**Exercise 363: Configure Email**  
**Goal:** Set your email  
**Task:** `git config --global user.email "you@example.com"`  
**Concept:** Email in commits  
**Help:** Match your GitHub email

**Exercise 364: View Config**  
**Goal:** Check settings  
**Task:** `git config --list`  
**Concept:** Shows all git settings  
**Help:** Verify your setup

**Exercise 365: Initialize Repository** ⭐  
**Goal:** Create new repo  
**Task:** `git init`  
**Concept:** Creates .git directory  
**Help:** Run in your project folder

**Exercise 366: Check Status** ⭐  
**Goal:** See repo status  
**Task:** `git status`  
**Concept:** Shows changes  
**Help:** Run this often!

**Exercise 367: Stage a File** ⭐  
**Goal:** Prepare for commit  
**Task:** `git add filename`  
**Concept:** Staging area  
**Help:** File ready to commit

**Exercise 368: Stage All Files**  
**Goal:** Add everything  
**Task:** `git add .`  
**Concept:** Dot means current directory  
**Help:** Be careful what you add!

**Exercise 369: First Commit** ⭐  
**Goal:** Save changes  
**Task:** `git commit -m "Initial commit"`  
**Concept:** Creates snapshot  
**Help:** `-m` for message

**Exercise 370: View History** ⭐  
**Goal:** See commits  
**Task:** `git log`  
**Concept:** Commit history  
**Help:** `--oneline` for brief view

---

### Week 38: Branching & Merging

**Exercise 371: Create Branch** ⭐  
**Goal:** New branch  
**Task:** `git branch feature-x`  
**Concept:** Branches are pointers  
**Help:** Doesn't switch to it

**Exercise 372: Switch Branch** ⭐  
**Goal:** Change branch  
**Task:** `git checkout feature-x`  
**Concept:** HEAD moves to branch  
**Help:** Or `git switch feature-x`

**Exercise 373: Create and Switch**  
**Goal:** One command  
**Task:** `git checkout -b feature-y`  
**Concept:** Create and switch  
**Help:** Common shortcut

**Exercise 374: List Branches**  
**Goal:** See all branches  
**Task:** `git branch`  
**Concept:** `*` marks current  
**Help:** `-a` shows remote too

**Exercise 375: Merge Branch** ⭐  
**Goal:** Combine branches  
**Task:** `git checkout main; git merge feature-x`  
**Concept:** Integrates changes  
**Help:** Must be on target branch

**Exercise 376: Delete Branch**  
**Goal:** Clean up  
**Task:** `git branch -d feature-x`  
**Concept:** Remove merged branch  
**Help:** `-D` forces delete

**Exercise 377: Merge Conflict** ⭐ 🎯  
**Goal:** Handle conflicts  
**Task:** Manually resolve conflict markers  
**Concept:** Same line changed  
**Help:** <<<<<<, ======, >>>>>>

**Exercise 378: Abort Merge**  
**Goal:** Cancel merge  
**Task:** `git merge --abort`  
**Concept:** Returns to pre-merge  
**Help:** When conflict too complex

**Exercise 379: Fast-Forward Merge**  
**Goal:** Understand FF  
**Task:** Merge with no divergence  
**Concept:** No merge commit needed  
**Help:** Linear history

**Exercise 380: No Fast-Forward**  
**Goal:** Force merge commit  
**Task:** `git merge --no-ff feature`  
**Concept:** Always creates merge commit  
**Help:** Better history visibility

---

### Week 39: Remote Repositories

**Exercise 381: Clone Repository** ⭐  
**Goal:** Copy remote repo  
**Task:** `git clone URL`  
**Concept:** Downloads entire repo  
**Help:** Creates new directory

**Exercise 382: View Remotes**  
**Goal:** See remote connections  
**Task:** `git remote -v`  
**Concept:** Shows fetch and push URLs  
**Help:** Usually origin

**Exercise 383: Add Remote**  
**Goal:** Connect to remote  
**Task:** `git remote add origin URL`  
**Concept:** Names remote connection  
**Help:** origin is conventional name

**Exercise 384: Fetch Changes** ⭐  
**Goal:** Download without merge  
**Task:** `git fetch origin`  
**Concept:** Gets remote changes  
**Help:** Doesn't modify working dir

**Exercise 385: Pull Changes** ⭐  
**Goal:** Download and merge  
**Task:** `git pull origin main`  
**Concept:** Fetch + merge  
**Help:** Updates current branch

**Exercise 386: Push Changes** ⭐  
**Goal:** Upload commits  
**Task:** `git push origin main`  
**Concept:** Sends to remote  
**Help:** Need permission

**Exercise 387: Push New Branch**  
**Goal:** Share branch  
**Task:** `git push -u origin feature-x`  
**Concept:** `-u` sets upstream  
**Help:** Tracks remote branch

**Exercise 388: Track Remote Branch**  
**Goal:** Follow remote  
**Task:** `git checkout --track origin/feature`  
**Concept:** Creates local tracking branch  
**Help:** For existing remote branches

**Exercise 389: Delete Remote Branch**  
**Goal:** Remove from remote  
**Task:** `git push origin --delete feature-x`  
**Concept:** Removes remote branch  
**Help:** Local branch remains

**Exercise 390: Prune Stale Branches**  
**Goal:** Clean remote tracking  
**Task:** `git fetch --prune`  
**Concept:** Removes deleted remote branches  
**Help:** Keep references clean

---

### Week 40: Advanced Git

**Exercise 391: Stash Changes** ⭐  
**Goal:** Temporarily save work  
**Task:** `git stash`  
**Concept:** Stores uncommitted changes  
**Help:** Working directory clean

**Exercise 392: Apply Stash**  
**Goal:** Restore stashed work  
**Task:** `git stash pop`  
**Concept:** Reapplies changes  
**Help:** `apply` keeps stash

**Exercise 393: List Stashes**  
**Goal:** See all stashes  
**Task:** `git stash list`  
**Concept:** Can have multiple  
**Help:** `stash@{0}` is latest

**Exercise 394: Cherry Pick**  
**Goal:** Copy single commit  
**Task:** `git cherry-pick commit-hash`  
**Concept:** Apply specific commit  
**Help:** Useful for hotfixes

**Exercise 395: Revert Commit**  
**Goal:** Undo with history  
**Task:** `git revert commit-hash`  
**Concept:** Creates undo commit  
**Help:** Safe for shared history

**Exercise 396: Reset Soft**  
**Goal:** Undo commit, keep changes  
**Task:** `git reset --soft HEAD~1`  
**Concept:** Moves HEAD, keeps staging  
**Help:** Uncommit but keep work

**Exercise 397: Reset Hard** ⚠️  
**Goal:** Completely undo  
**Task:** `git reset --hard HEAD~1`  
**Concept:** Discards changes  
**Warning:** Cannot recover!

**Exercise 398: Rebase** ⭐  
**Goal:** Linear history  
**Task:** `git rebase main`  
**Concept:** Replays commits  
**Help:** Don't rebase public branches!

**Exercise 399: Interactive Rebase**  
**Goal:** Edit history  
**Task:** `git rebase -i HEAD~3`  
**Concept:** Squash, reorder, edit  
**Help:** Powerful but careful!

**Exercise 400: Git Bisect** 📝  
**Goal:** Find bug introduction  
**Task:** `git bisect start`, mark good/bad  
**Concept:** Binary search commits  
**Help:** Find which commit broke things

---

### Week 41: Git Workflows

**Exercise 401: Gitignore File** ⭐  
**Goal:** Ignore files  
**Task:** Create `.gitignore`  
**Concept:** Patterns to exclude  
**Help:** `*.log`, `node_modules/`

**Exercise 402: Global Gitignore**  
**Goal:** Always ignore  
**Task:** Configure global gitignore  
**Concept:** Personal ignores  
**Help:** IDE files, OS files

**Exercise 403: Git Tags** ⭐  
**Goal:** Mark releases  
**Task:** `git tag v1.0.0`  
**Concept:** Named reference to commit  
**Help:** For version releases

**Exercise 404: Annotated Tags**  
**Goal:** Tag with message  
**Task:** `git tag -a v1.0.0 -m "Release 1.0"`  
**Concept:** More information  
**Help:** Recommended for releases

**Exercise 405: Push Tags**  
**Goal:** Share tags  
**Task:** `git push --tags`  
**Concept:** Tags don't push automatically  
**Help:** Or push single tag

**Exercise 406: Git Blame**  
**Goal:** Find who changed line  
**Task:** `git blame filename`  
**Concept:** Shows line-by-line author  
**Help:** Track down changes

**Exercise 407: Git Diff** ⭐  
**Goal:** See changes  
**Task:** `git diff`  
**Concept:** Shows modifications  
**Help:** `--staged` for staged changes

**Exercise 408: Diff Between Branches**  
**Goal:** Compare branches  
**Task:** `git diff main..feature`  
**Concept:** Shows difference  
**Help:** What feature adds

**Exercise 409: Git Log Graph**  
**Goal:** Visual history  
**Task:** `git log --graph --oneline`  
**Concept:** Shows branching  
**Help:** `--all` shows all branches

**Exercise 410: Git Hooks** ⭐  
**Goal:** Automated actions  
**Task:** Create `.git/hooks/pre-commit`  
**Concept:** Scripts run at events  
**Help:** Lint before commit

---

### Week 42: Collaborative Git

**Exercise 411: Fork Workflow**  
**Goal:** Contribute to others  
**Task:** Fork, clone, branch, PR  
**Concept:** Standard open source flow  
**Help:** Fork is your copy

**Exercise 412: Upstream Remote**  
**Goal:** Track original repo  
**Task:** `git remote add upstream URL`  
**Concept:** Sync with original  
**Help:** Pull from upstream

**Exercise 413: Sync Fork**  
**Goal:** Update your fork  
**Task:** `git fetch upstream; git merge upstream/main`  
**Concept:** Keep fork current  
**Help:** Do regularly

**Exercise 414: Pull Request** ⭐  
**Goal:** Request merge  
**Task:** Create PR on GitHub  
**Concept:** Code review process  
**Help:** Push branch, create PR

**Exercise 415: Code Review**  
**Goal:** Review changes  
**Task:** Comment on PR  
**Concept:** Quality control  
**Help:** Approve or request changes

**Exercise 416: Squash Merge**  
**Goal:** Clean history  
**Task:** Squash when merging PR  
**Concept:** Combines commits  
**Help:** One commit per PR

**Exercise 417: Rebase and Merge**  
**Goal:** Linear history  
**Task:** Rebase before merge  
**Concept:** No merge commits  
**Help:** Clean but loses context

**Exercise 418: Conventional Commits** ⭐  
**Goal:** Commit message format  
**Task:** Use `feat:`, `fix:`, `docs:` prefixes  
**Concept:** Standardized messages  
**Help:** Enables automation

**Exercise 419: Semantic Versioning** ⭐  
**Goal:** Version numbers  
**Task:** Understand MAJOR.MINOR.PATCH  
**Concept:** Meaningful versions  
**Help:** Breaking.Feature.Fix

**Exercise 420: Git Workflow Document** 📝  
**Goal:** Define team workflow  
**Task:** Document branching strategy  
**Concept:** Consistent process  
**Help:** Git Flow, GitHub Flow, Trunk-based

---

## ⚙️ PHASE 8: CI/CD Pipelines (Exercises 421-480)

### Week 43: CI/CD Concepts

**Exercise 421: Understand CI** ⭐  
**Goal:** What is Continuous Integration  
**Task:** Research and document  
**Concept:** Merge frequently, test automatically  
**Help:** Small, frequent commits

**Exercise 422: Understand CD** ⭐  
**Goal:** Continuous Delivery/Deployment  
**Task:** Know the difference  
**Concept:** Delivery = can deploy, Deployment = auto deploy  
**Help:** CD builds on CI

**Exercise 423: Pipeline Stages**  
**Goal:** Typical pipeline structure  
**Task:** Document: build, test, deploy  
**Concept:** Sequential stages  
**Help:** Each stage has jobs

**Exercise 424: Artifacts**  
**Goal:** Build outputs  
**Task:** Understand what artifacts are  
**Concept:** Files passed between stages  
**Help:** Built code, test reports

**Exercise 425: Install Jenkins** ⭐  
**Goal:** Set up Jenkins locally  
**Task:** Run Jenkins with Docker  
**Concept:** Popular CI/CD server  
**Help:** `docker run -p 8080:8080 jenkins/jenkins`

**Exercise 426: Jenkins Initial Setup**  
**Goal:** First-time configuration  
**Task:** Get admin password, install plugins  
**Concept:** Setup wizard  
**Help:** Password in logs

**Exercise 427: Create Jenkins Job** ⭐  
**Goal:** First pipeline  
**Task:** New Item → Freestyle project  
**Concept:** Jobs are units of work  
**Help:** Start simple

**Exercise 428: Build Step**  
**Goal:** Add shell command  
**Task:** Execute shell: `echo "Hello Jenkins"`  
**Concept:** Build steps run commands  
**Help:** Build → Execute shell

**Exercise 429: Trigger Build**  
**Goal:** Run job manually  
**Task:** Click "Build Now"  
**Concept:** Manual trigger  
**Help:** Watch console output

**Exercise 430: View Console Output**  
**Goal:** See build logs  
**Task:** Click build number → Console Output  
**Concept:** Debug builds here  
**Help:** Shows all output

---

### Week 44: Jenkins Pipelines

**Exercise 431: Pipeline Job** ⭐  
**Goal:** Create pipeline  
**Task:** New Item → Pipeline  
**Concept:** Pipelines as code  
**Help:** Uses Jenkinsfile syntax

**Exercise 432: Declarative Pipeline** ⭐  
**Goal:** Modern pipeline syntax  
**Task:** Write pipeline with `pipeline { }`  
**Concept:** Structured, readable  
**Help:** Starts with `pipeline {`

**Exercise 433: Pipeline Agent**  
**Goal:** Where to run  
**Task:** `agent any`  
**Concept:** Defines execution environment  
**Help:** `any` = any available agent

**Exercise 434: Pipeline Stages** ⭐  
**Goal:** Define stages  
**Task:** `stages { stage('Build') { } }`  
**Concept:** Logical groupings  
**Help:** Named stages

**Exercise 435: Pipeline Steps**  
**Goal:** Commands in stages  
**Task:** `steps { sh 'echo hello' }`  
**Concept:** Actual work  
**Help:** `sh` runs shell commands

**Exercise 436: Multi-Stage Pipeline**  
**Goal:** Build, Test, Deploy  
**Task:** Three stages in pipeline  
**Concept:** Sequential execution  
**Help:** Stages run in order

**Exercise 437: Jenkinsfile** ⭐  
**Goal:** Pipeline in repo  
**Task:** Create `Jenkinsfile` in project  
**Concept:** Pipeline as code  
**Help:** Version controlled

**Exercise 438: Pipeline from SCM**  
**Goal:** Load from repo  
**Task:** Pipeline → Definition → Pipeline script from SCM  
**Concept:** Git integration  
**Help:** Points to your repo

**Exercise 439: Environment Variables**  
**Goal:** Set variables  
**Task:** `environment { MY_VAR = 'value' }`  
**Concept:** Available to all steps  
**Help:** Access with `$MY_VAR`

**Exercise 440: Credentials** ⭐  
**Goal:** Secure secrets  
**Task:** Add credential in Jenkins  
**Concept:** Don't hardcode secrets!  
**Help:** Manage Jenkins → Credentials

---

### Week 45: Advanced Jenkins

**Exercise 441: Pipeline Parameters**  
**Goal:** Input to pipeline  
**Task:** `parameters { string(...) }`  
**Concept:** Configurable builds  
**Help:** Build with Parameters

**Exercise 442: Conditional Execution**  
**Goal:** Run stage conditionally  
**Task:** `when { branch 'main' }`  
**Concept:** Skip stages  
**Help:** Only on certain conditions

**Exercise 443: Post Actions**  
**Goal:** Always run  
**Task:** `post { always { ... } }`  
**Concept:** Cleanup, notifications  
**Help:** success, failure, always

**Exercise 444: Parallel Stages**  
**Goal:** Run simultaneously  
**Task:** `parallel { stage('A') {} stage('B') {} }`  
**Concept:** Speed up pipeline  
**Help:** Independent stages

**Exercise 445: Pipeline Timeout**  
**Goal:** Prevent hanging  
**Task:** `options { timeout(time: 1, unit: 'HOURS') }`  
**Concept:** Kill stuck builds  
**Help:** At pipeline or stage level

**Exercise 446: Archive Artifacts**  
**Goal:** Save build outputs  
**Task:** `archiveArtifacts artifacts: '*.jar'`  
**Concept:** Available after build  
**Help:** Download from UI

**Exercise 447: Publish Test Results**  
**Goal:** Show test reports  
**Task:** `junit '**/test-results/*.xml'`  
**Concept:** Test visibility  
**Help:** JUnit format

**Exercise 448: Input Step**  
**Goal:** Manual approval  
**Task:** `input message: 'Deploy?'`  
**Concept:** Pause for approval  
**Help:** Human gate

**Exercise 449: Shared Libraries**  
**Goal:** Reusable code  
**Task:** Create shared library  
**Concept:** DRY for pipelines  
**Help:** @Library annotation

**Exercise 450: Webhooks** ⭐  
**Goal:** Auto trigger  
**Task:** Configure GitHub webhook  
**Concept:** Push triggers build  
**Help:** GitHub → Webhooks

---

### Week 46: GitLab CI/CD

**Exercise 451: GitLab CI Introduction** ⭐  
**Goal:** Alternative CI system  
**Task:** Understand GitLab CI  
**Concept:** Built into GitLab  
**Help:** No separate server

**Exercise 452: Create .gitlab-ci.yml** ⭐  
**Goal:** Pipeline definition  
**Task:** Create file in repo root  
**Concept:** YAML configuration  
**Help:** Similar to compose

**Exercise 453: Basic Job**  
**Goal:** First GitLab job  
**Task:** Define job with script  
**Concept:** Jobs are basic units  
**Help:** `job_name: script: [...]`

**Exercise 454: Stages Definition**  
**Goal:** Define pipeline stages  
**Task:** `stages: [build, test, deploy]`  
**Concept:** Runs in order  
**Help:** Jobs in same stage parallel

**Exercise 455: Job Stage Assignment**  
**Goal:** Assign job to stage  
**Task:** `stage: build`  
**Concept:** Controls execution order  
**Help:** Default is test

**Exercise 456: Docker Image**  
**Goal:** Run job in container  
**Task:** `image: python:3.11`  
**Concept:** Clean environment  
**Help:** Any Docker image

**Exercise 457: Cache Dependencies**  
**Goal:** Speed up builds  
**Task:** Configure cache  
**Concept:** Preserve between runs  
**Help:** `cache: paths: [...]`

**Exercise 458: Artifacts in GitLab**  
**Goal:** Pass files between jobs  
**Task:** `artifacts: paths: [...]`  
**Concept:** Available downstream  
**Help:** Download from UI

**Exercise 459: Rules and Conditions**  
**Goal:** Conditional jobs  
**Task:** `rules: - if: ...`  
**Concept:** When to run  
**Help:** More flexible than only

**Exercise 460: Variables in GitLab**  
**Goal:** Configuration values  
**Task:** `variables: KEY: value`  
**Concept:** Available in scripts  
**Help:** Can be protected/masked

---

### Week 47: GitHub Actions

**Exercise 461: GitHub Actions Intro** ⭐  
**Goal:** GitHub's CI/CD  
**Task:** Understand Actions  
**Concept:** Native GitHub integration  
**Help:** Built into GitHub

**Exercise 462: Create Workflow** ⭐  
**Goal:** First workflow  
**Task:** Create `.github/workflows/main.yml`  
**Concept:** Workflows in repo  
**Help:** Directory matters!

**Exercise 463: Workflow Name**  
**Goal:** Identify workflow  
**Task:** `name: CI Pipeline`  
**Concept:** Shows in UI  
**Help:** Descriptive names

**Exercise 464: Trigger Events** ⭐  
**Goal:** When to run  
**Task:** `on: [push, pull_request]`  
**Concept:** Event-driven  
**Help:** Many event types

**Exercise 465: Define Jobs**  
**Goal:** Job structure  
**Task:** `jobs: build: ...`  
**Concept:** Jobs run in parallel  
**Help:** Can have dependencies

**Exercise 466: Runs-On**  
**Goal:** Runner type  
**Task:** `runs-on: ubuntu-latest`  
**Concept:** Where job runs  
**Help:** ubuntu, windows, macos

**Exercise 467: Job Steps**  
**Goal:** Steps in job  
**Task:** `steps: - name: ... run: ...`  
**Concept:** Sequential commands  
**Help:** Each step is one action

**Exercise 468: Using Actions** ⭐  
**Goal:** Pre-built actions  
**Task:** `uses: actions/checkout@v4`  
**Concept:** Reusable actions  
**Help:** Marketplace has many

**Exercise 469: Checkout Code**  
**Goal:** Get code  
**Task:** Use `actions/checkout`  
**Concept:** Required to access repo  
**Help:** Usually first step

**Exercise 470: Setup Language**  
**Goal:** Configure runtime  
**Task:** `actions/setup-node@v4`  
**Concept:** Install language version  
**Help:** Node, Python, Java, etc.

---

### Week 48: CI/CD Best Practices

**Exercise 471: Run Tests** ⭐  
**Goal:** Automated testing  
**Task:** Add test step to pipeline  
**Concept:** Catch bugs early  
**Help:** `npm test`, `pytest`, etc.

**Exercise 472: Code Linting**  
**Goal:** Style checking  
**Task:** Run linter in pipeline  
**Concept:** Consistent code style  
**Help:** ESLint, Flake8, etc.

**Exercise 473: Security Scanning**  
**Goal:** Find vulnerabilities  
**Task:** Add security scan  
**Concept:** Shift left security  
**Help:** Trivy, Snyk, etc.

**Exercise 474: Build Docker Image**  
**Goal:** Create container  
**Task:** `docker build` in pipeline  
**Concept:** Containerized artifacts  
**Help:** Tag with commit SHA

**Exercise 475: Push to Registry**  
**Goal:** Store image  
**Task:** Push to local registry  
**Concept:** Image distribution  
**Help:** Login then push

**Exercise 476: Deploy Stage** ⭐  
**Goal:** Automate deployment  
**Task:** Add deploy stage  
**Concept:** Continuous Deployment  
**Help:** After tests pass

**Exercise 477: Environment Protection**  
**Goal:** Approval for prod  
**Task:** Require approval  
**Concept:** Manual gate  
**Help:** Prevent accidents

**Exercise 478: Rollback Strategy**  
**Goal:** Plan for failure  
**Task:** Document rollback process  
**Concept:** Quick recovery  
**Help:** Previous version ready

**Exercise 479: Pipeline Optimization**  
**Goal:** Speed up pipeline  
**Task:** Parallelize, cache  
**Concept:** Fast feedback  
**Help:** Minutes not hours

**Exercise 480: CI/CD Documentation** 📝  
**Goal:** Document pipeline  
**Task:** README for pipeline  
**Concept:** Team knowledge  
**Help:** How to run, debug

---

## 🏗️ PHASE 9: Infrastructure as Code (Exercises 481-540)

### Week 49: IaC Concepts

**Exercise 481: Understand IaC** ⭐  
**Goal:** What is Infrastructure as Code  
**Task:** Research and document  
**Concept:** Manage infra like code  
**Help:** Version controlled, reproducible

**Exercise 482: Benefits of IaC**  
**Goal:** Why use IaC  
**Task:** List benefits  
**Concept:** Consistency, speed, documentation  
**Help:** No manual configuration

**Exercise 483: Declarative vs Imperative**  
**Goal:** Two approaches  
**Task:** Understand difference  
**Concept:** What vs How  
**Help:** Terraform = declarative

**Exercise 484: Idempotency** ⭐  
**Goal:** Key concept  
**Task:** Understand idempotent operations  
**Concept:** Same result every run  
**Help:** Apply multiple times safely

**Exercise 485: State Management**  
**Goal:** Track infrastructure  
**Task:** Understand state concept  
**Concept:** What exists currently  
**Help:** Needed for changes

**Exercise 486: Ansible Introduction** ⭐  
**Goal:** Configuration management  
**Task:** Understand Ansible  
**Concept:** Agentless automation  
**Help:** SSH-based, no agent

**Exercise 487: Install Ansible**  
**Goal:** Set up Ansible  
**Task:** `pip install ansible`  
**Concept:** Python-based tool  
**Help:** Or `apt install ansible`

**Exercise 488: Ansible Inventory** ⭐  
**Goal:** Define hosts  
**Task:** Create inventory file  
**Concept:** Hosts and groups  
**Help:** INI or YAML format

**Exercise 489: Simple Inventory**  
**Goal:** Local testing  
**Task:** `localhost ansible_connection=local`  
**Concept:** Test on local machine  
**Help:** No SSH needed

**Exercise 490: Ansible Ad-Hoc** ⭐  
**Goal:** Quick commands  
**Task:** `ansible all -m ping`  
**Concept:** One-off tasks  
**Help:** `-m` specifies module

---

### Week 50: Ansible Playbooks

**Exercise 491: First Playbook** ⭐  
**Goal:** Write playbook  
**Task:** Create YAML playbook  
**Concept:** Playbooks are automation  
**Help:** `---` starts YAML

**Exercise 492: Playbook Structure**  
**Goal:** Understand format  
**Task:** hosts, tasks, name  
**Concept:** YAML structure  
**Help:** Indentation matters!

**Exercise 493: Run Playbook** ⭐  
**Goal:** Execute playbook  
**Task:** `ansible-playbook playbook.yml`  
**Concept:** Runs all tasks  
**Help:** `-v` for verbose

**Exercise 494: Task with Module**  
**Goal:** Use Ansible module  
**Task:** Use `file` module  
**Concept:** Modules do work  
**Help:** `state: directory`

**Exercise 495: Install Package** ⭐  
**Goal:** Manage packages  
**Task:** Use `apt` module  
**Concept:** Package management  
**Help:** `state: present`

**Exercise 496: Copy File**  
**Goal:** Deploy files  
**Task:** Use `copy` module  
**Concept:** File distribution  
**Help:** `src` and `dest`

**Exercise 497: Template Module** ⭐  
**Goal:** Dynamic files  
**Task:** Use `template` module  
**Concept:** Jinja2 templates  
**Help:** Variables in files

**Exercise 498: Service Module**  
**Goal:** Manage services  
**Task:** `service: name=nginx state=started`  
**Concept:** Control services  
**Help:** `enabled: yes` for boot

**Exercise 499: Handlers** ⭐  
**Goal:** Triggered tasks  
**Task:** Create handler for restart  
**Concept:** Run only when notified  
**Help:** `notify: handler_name`

**Exercise 500: Variables in Playbook**  
**Goal:** Use variables  
**Task:** Define `vars:` section  
**Concept:** Parameterize playbooks  
**Help:** Access with `{{ var }}`

---

### Week 51: Advanced Ansible

**Exercise 501: Conditionals**  
**Goal:** When to run task  
**Task:** Use `when:` condition  
**Concept:** Conditional execution  
**Help:** `when: ansible_os_family == "Debian"`

**Exercise 502: Loops**  
**Goal:** Repeat task  
**Task:** Use `loop:` or `with_items:`  
**Concept:** Iterate over list  
**Help:** `{{ item }}` in task

**Exercise 503: Register Output**  
**Goal:** Capture result  
**Task:** `register: result`  
**Concept:** Use output later  
**Help:** Access `result.stdout`

**Exercise 504: Include Tasks**  
**Goal:** Organize playbooks  
**Task:** `include_tasks: file.yml`  
**Concept:** Modular playbooks  
**Help:** Reuse task files

**Exercise 505: Roles** ⭐  
**Goal:** Reusable components  
**Task:** Create role structure  
**Concept:** tasks, handlers, defaults  
**Help:** `ansible-galaxy init role_name`

**Exercise 506: Role Directory Structure**  
**Goal:** Understand layout  
**Task:** Create tasks/main.yml  
**Concept:** Standard structure  
**Help:** defaults, vars, templates

**Exercise 507: Use Role in Playbook**  
**Goal:** Apply role  
**Task:** `roles: - role_name`  
**Concept:** Include role  
**Help:** From roles/ directory

**Exercise 508: Ansible Galaxy**  
**Goal:** Community roles  
**Task:** `ansible-galaxy install role`  
**Concept:** Pre-built roles  
**Help:** Saves time

**Exercise 509: Ansible Vault** ⭐  
**Goal:** Encrypt secrets  
**Task:** `ansible-vault encrypt file`  
**Concept:** Secure sensitive data  
**Help:** `--ask-vault-pass`

**Exercise 510: Vault in Playbook**  
**Goal:** Use encrypted vars  
**Task:** Include vault file  
**Concept:** Decrypt at runtime  
**Help:** Variables work normally

---

### Week 52: Terraform Basics (Local)

**Exercise 511: Install Terraform** ⭐  
**Goal:** Set up Terraform  
**Task:** Download and install  
**Concept:** IaC tool  
**Help:** Add to PATH

**Exercise 512: Terraform Version**  
**Goal:** Verify installation  
**Task:** `terraform version`  
**Concept:** Check setup  
**Help:** Should show version

**Exercise 513: First Configuration** ⭐  
**Goal:** Write Terraform config  
**Task:** Create `main.tf`  
**Concept:** HCL language  
**Help:** HashiCorp Configuration Language

**Exercise 514: Local File Provider**  
**Goal:** Practice without cloud  
**Task:** Use local provider  
**Concept:** Manage local files  
**Help:** Great for learning

**Exercise 515: Terraform Init** ⭐  
**Goal:** Initialize project  
**Task:** `terraform init`  
**Concept:** Downloads providers  
**Help:** Run in config directory

**Exercise 516: Terraform Plan** ⭐  
**Goal:** Preview changes  
**Task:** `terraform plan`  
**Concept:** Dry run  
**Help:** See what will happen

**Exercise 517: Terraform Apply** ⭐  
**Goal:** Create resources  
**Task:** `terraform apply`  
**Concept:** Execute changes  
**Help:** Confirm with `yes`

**Exercise 518: Terraform State**  
**Goal:** Understand state file  
**Task:** View `terraform.tfstate`  
**Concept:** Tracks what exists  
**Help:** Don't edit manually!

**Exercise 519: Terraform Destroy** ⭐  
**Goal:** Remove resources  
**Task:** `terraform destroy`  
**Concept:** Tear down  
**Help:** Clean up

**Exercise 520: Variables in Terraform**  
**Goal:** Parameterize config  
**Task:** Define `variable` block  
**Concept:** Reusable configs  
**Help:** `var.variable_name`

---

### Week 53: More Terraform

**Exercise 521: Variable Types**  
**Goal:** String, number, list, map  
**Task:** Define different types  
**Concept:** Type constraints  
**Help:** `type = string`

**Exercise 522: Variable Defaults**  
**Goal:** Default values  
**Task:** `default = "value"`  
**Concept:** Optional input  
**Help:** Override when needed

**Exercise 523: Variable Files**  
**Goal:** Separate variables  
**Task:** Create `terraform.tfvars`  
**Concept:** Values separate from config  
**Help:** Automatically loaded

**Exercise 524: Outputs**  
**Goal:** Display information  
**Task:** Define `output` block  
**Concept:** Expose values  
**Help:** Shown after apply

**Exercise 525: Data Sources**  
**Goal:** Read existing resources  
**Task:** Use `data` block  
**Concept:** Reference external data  
**Help:** Read, not create

**Exercise 526: Local Values**  
**Goal:** Computed values  
**Task:** `locals { ... }`  
**Concept:** Reusable expressions  
**Help:** `local.name`

**Exercise 527: Resource Dependencies**  
**Goal:** Control order  
**Task:** Implicit vs explicit  
**Concept:** Terraform figures out order  
**Help:** `depends_on` if needed

**Exercise 528: Count**  
**Goal:** Multiple instances  
**Task:** `count = 3`  
**Concept:** Create several  
**Help:** `count.index`

**Exercise 529: For Each**  
**Goal:** Iterate over map  
**Task:** `for_each = var.map`  
**Concept:** More flexible than count  
**Help:** `each.key`, `each.value`

**Exercise 530: Modules** ⭐  
**Goal:** Reusable components  
**Task:** Create module directory  
**Concept:** Encapsulate resources  
**Help:** Like functions

---

### Week 54: IaC Best Practices

**Exercise 531: Use Module**  
**Goal:** Call module  
**Task:** `module "name" { source = "./modules/x" }`  
**Concept:** Reuse modules  
**Help:** Pass variables

**Exercise 532: Module Outputs**  
**Goal:** Get values from module  
**Task:** Access `module.name.output`  
**Concept:** Inter-module communication  
**Help:** Define outputs in module

**Exercise 533: Terraform Format**  
**Goal:** Consistent style  
**Task:** `terraform fmt`  
**Concept:** Auto-format code  
**Help:** Run before commit

**Exercise 534: Terraform Validate**  
**Goal:** Check configuration  
**Task:** `terraform validate`  
**Concept:** Syntax validation  
**Help:** Catches errors early

**Exercise 535: State Locking**  
**Goal:** Prevent conflicts  
**Task:** Understand locking  
**Concept:** One change at a time  
**Help:** Remote state enables

**Exercise 536: Workspaces**  
**Goal:** Multiple environments  
**Task:** `terraform workspace new dev`  
**Concept:** Separate state per env  
**Help:** dev, staging, prod

**Exercise 537: Drift Detection**  
**Goal:** Find manual changes  
**Task:** `terraform plan` to detect  
**Concept:** Config vs reality  
**Help:** State mismatch

**Exercise 538: Import Resources**  
**Goal:** Adopt existing  
**Task:** `terraform import`  
**Concept:** Bring into state  
**Help:** For existing resources

**Exercise 539: Sensitive Variables**  
**Goal:** Hide secrets  
**Task:** `sensitive = true`  
**Concept:** Don't show in output  
**Help:** Still in state file!

**Exercise 540: IaC Review Process** 📝  
**Goal:** Safe changes  
**Task:** Plan → Review → Apply  
**Concept:** Always review plans  
**Help:** Like code review

---

## 🛡️ PHASE 10: Security & Best Practices (Exercises 541-600)

### Week 55: Security Fundamentals

**Exercise 541: Least Privilege** ⭐  
**Goal:** Minimal permissions  
**Task:** Understand principle  
**Concept:** Only needed access  
**Help:** Reduce attack surface

**Exercise 542: Check Open Ports**  
**Goal:** Security audit  
**Task:** `ss -tlnp` and review  
**Concept:** Close unnecessary ports  
**Help:** Each open port is risk

**Exercise 543: Disable Root Login** ⭐  
**Goal:** Secure SSH  
**Task:** Set `PermitRootLogin no` in sshd_config  
**Concept:** Force user accounts  
**Help:** Use sudo instead

**Exercise 544: SSH Key Only**  
**Goal:** No password auth  
**Task:** `PasswordAuthentication no`  
**Concept:** Keys more secure  
**Help:** After setting up keys!

**Exercise 545: Fail2ban Setup** ⭐  
**Goal:** Block brute force  
**Task:** Install and configure fail2ban  
**Concept:** Auto-block attackers  
**Help:** Monitors auth log

**Exercise 546: System Updates** ⭐  
**Goal:** Keep patched  
**Task:** Regular `apt update && apt upgrade`  
**Concept:** Security patches  
**Help:** Automate with unattended-upgrades

**Exercise 547: Check for Vulnerabilities**  
**Goal:** Security scanning  
**Task:** Use `lynis audit system`  
**Concept:** Find weaknesses  
**Help:** Install lynis first

**Exercise 548: File Permissions Audit**  
**Goal:** Find insecure files  
**Task:** `find / -perm -777 -type f`  
**Concept:** World-writable is risky  
**Help:** Fix or justify each

**Exercise 549: SUID Files**  
**Goal:** Find privileged files  
**Task:** `find / -perm -4000 -type f`  
**Concept:** SUID can be exploited  
**Help:** Minimize SUID files

**Exercise 550: User Password Policy**  
**Goal:** Strong passwords  
**Task:** Configure PAM  
**Concept:** Complexity requirements  
**

**Help:** `/etc/pam.d/common-password`

---

### Week 56: Container Security

**Exercise 551: Non-Root Containers** ⭐  
**Goal:** Run as non-root user  
**Task:** Add `USER` instruction in Dockerfile  
**Concept:** Limit container privileges  
**Help:** `USER 1000` or `USER appuser`

**Exercise 552: Read-Only Filesystem**  
**Goal:** Immutable containers  
**Task:** `docker run --read-only nginx`  
**Concept:** Prevent writes  
**Help:** Add tmpfs for needed writes

**Exercise 553: Drop Capabilities**  
**Goal:** Remove kernel capabilities  
**Task:** `--cap-drop ALL --cap-add NET_BIND_SERVICE`  
**Concept:** Minimal privileges  
**Help:** Only add what's needed

**Exercise 554: Scan Images** ⭐  
**Goal:** Find vulnerabilities  
**Task:** `docker scan imagename` or use Trivy  
**Concept:** Known CVEs in images  
**Help:** `trivy image nginx`

**Exercise 555: Use Minimal Base Images**  
**Goal:** Reduce attack surface  
**Task:** Use `alpine` or `distroless`  
**Concept:** Fewer packages = fewer vulnerabilities  
**Help:** `FROM python:3.11-alpine`

**Exercise 556: No Latest Tag** ⭐  
**Goal:** Predictable images  
**Task:** Use specific version tags  
**Concept:** `latest` changes unpredictably  
**Help:** `nginx:1.24.0` not `nginx:latest`

**Exercise 557: Docker Content Trust**  
**Goal:** Verify image signatures  
**Task:** `export DOCKER_CONTENT_TRUST=1`  
**Concept:** Only signed images  
**Help:** Prevents tampering

**Exercise 558: Secrets Management** ⭐  
**Goal:** Don't hardcode secrets  
**Task:** Use Docker secrets or env vars  
**Concept:** Separate secrets from code  
**Help:** Never in Dockerfile!

**Exercise 559: Network Segmentation**  
**Goal:** Isolate containers  
**Task:** Create separate networks  
**Concept:** Limit communication  
**Help:** Only connect what's needed

**Exercise 560: Resource Limits** ⭐  
**Goal:** Prevent resource exhaustion  
**Task:** `--memory=512m --cpus=0.5`  
**Concept:** Container can't consume all  
**Help:** Protects host and other containers

---

### Week 57: Secrets Management

**Exercise 561: Environment Variables**  
**Goal:** Basic secret passing  
**Task:** Use `-e SECRET=value`  
**Concept:** Runtime configuration  
**Help:** Better than hardcoding

**Exercise 562: Env File** ⭐  
**Goal:** File-based secrets  
**Task:** `--env-file .env`  
**Concept:** Keep secrets in file  
**Help:** Don't commit .env!

**Exercise 563: Docker Secrets**  
**Goal:** Swarm secrets  
**Task:** `docker secret create`  
**Concept:** Encrypted at rest  
**Help:** Available in /run/secrets/

**Exercise 564: HashiCorp Vault Intro** ⭐  
**Goal:** Secrets management tool  
**Task:** Understand Vault concepts  
**Concept:** Centralized secrets  
**Help:** Dynamic secrets, leasing

**Exercise 565: Install Vault**  
**Goal:** Run Vault locally  
**Task:** Run Vault dev server  
**Concept:** Development mode  
**Help:** `vault server -dev`

**Exercise 566: Vault CLI**  
**Goal:** Interact with Vault  
**Task:** `vault status`  
**Concept:** CLI for operations  
**Help:** Set VAULT_ADDR first

**Exercise 567: Store Secret in Vault**  
**Goal:** Write secret  
**Task:** `vault kv put secret/myapp password=secret123`  
**Concept:** Key-value store  
**Help:** KV secrets engine

**Exercise 568: Read Secret from Vault**  
**Goal:** Retrieve secret  
**Task:** `vault kv get secret/myapp`  
**Concept:** Fetch at runtime  
**Help:** `-field=password` for specific

**Exercise 569: Vault in Scripts**  
**Goal:** Automate secret retrieval  
**Task:** Use vault CLI in script  
**Concept:** No hardcoded secrets  
**Help:** `PASSWORD=$(vault kv get -field=password secret/myapp)`

**Exercise 570: Git Secrets** ⭐  
**Goal:** Prevent secret commits  
**Task:** Install and configure git-secrets  
**Concept:** Pre-commit hook  
**Help:** Blocks commits with secrets

---

### Week 58: Backup & Recovery

**Exercise 571: Backup Strategy** ⭐  
**Goal:** Plan backups  
**Task:** Document 3-2-1 rule  
**Concept:** 3 copies, 2 media, 1 offsite  
**Help:** Foundation of data safety

**Exercise 572: Tar Backup**  
**Goal:** Create archive  
**Task:** `tar -czvf backup.tar.gz /data`  
**Concept:** Compress and archive  
**Help:** `-c` create, `-z` gzip, `-v` verbose

**Exercise 573: Incremental Backup**  
**Goal:** Only changed files  
**Task:** Use `rsync` for incremental  
**Concept:** Faster subsequent backups  
**Help:** `rsync -av --delete`

**Exercise 574: Database Backup** ⭐  
**Goal:** Backup database  
**Task:** `pg_dump` or `mysqldump`  
**Concept:** Consistent database copy  
**Help:** `pg_dump dbname > backup.sql`

**Exercise 575: Scheduled Backups**  
**Goal:** Automate backups  
**Task:** Cron job for backup script  
**Concept:** Regular, automatic  
**Help:** Daily at 2 AM

**Exercise 576: Backup Rotation**  
**Goal:** Manage backup files  
**Task:** Keep 7 daily, 4 weekly  
**Concept:** Don't fill disk  
**Help:** Delete old backups

**Exercise 577: Test Restore** ⭐ 🎯  
**Goal:** Verify backups work  
**Task:** Actually restore from backup  
**Concept:** Untested backup = no backup  
**Help:** Do this regularly!

**Exercise 578: Docker Volume Backup**  
**Goal:** Backup container data  
**Task:** Backup named volumes  
**Concept:** Data outlives containers  
**Help:** Mount volume, tar contents

**Exercise 579: Configuration Backup**  
**Goal:** Save system config  
**Task:** Backup /etc directory  
**Concept:** Reproduce system  
**Help:** `tar -czvf etc-backup.tar.gz /etc`

**Exercise 580: Disaster Recovery Plan** 📝  
**Goal:** Document recovery  
**Task:** Write recovery procedures  
**Concept:** Step-by-step restoration  
**Help:** RTO and RPO defined

---

### Week 59: Performance & Troubleshooting

**Exercise 581: Identify Bottleneck** ⭐  
**Goal:** Find slow component  
**Task:** Check CPU, memory, disk, network  
**Concept:** Systematic approach  
**Help:** One is usually the limit

**Exercise 582: High CPU Investigation**  
**Goal:** Find CPU hog  
**Task:** `top` or `htop`, sort by CPU  
**Concept:** Identify process  
**Help:** `ps aux --sort=-%cpu`

**Exercise 583: Memory Investigation**  
**Goal:** Find memory hog  
**Task:** Sort by memory usage  
**Concept:** Identify process  
**Help:** `ps aux --sort=-%mem`

**Exercise 584: Disk I/O Investigation**  
**Goal:** Find I/O bottleneck  
**Task:** `iotop` to see disk usage  
**Concept:** Which process uses disk  
**Help:** `sudo iotop -o` shows active only

**Exercise 585: Network Investigation**  
**Goal:** Find network issues  
**Task:** `iftop` or `nethogs`  
**Concept:** Bandwidth usage  
**Help:** Per-process network

**Exercise 586: Strace** ⭐  
**Goal:** Trace system calls  
**Task:** `strace -p PID`  
**Concept:** See what process does  
**Help:** Great for debugging

**Exercise 587: Lsof** ⭐  
**Goal:** List open files  
**Task:** `lsof -p PID`  
**Concept:** Files, sockets, connections  
**Help:** What process accesses

**Exercise 588: Container Debugging**  
**Goal:** Debug running container  
**Task:** `docker exec -it container sh`  
**Concept:** Get inside container  
**Help:** Install debug tools if needed

**Exercise 589: Container Logs**  
**Goal:** Troubleshoot container  
**Task:** `docker logs --tail 100 -f container`  
**Concept:** Application output  
**Help:** Last 100 lines, follow

**Exercise 590: Core Dump Analysis**  
**Goal:** Debug crashes  
**Task:** Enable core dumps  
**Concept:** Post-mortem debugging  
**Help:** `ulimit -c unlimited`

---

### Week 60: DevOps Culture & Final Projects

**Exercise 591: DevOps Principles** ⭐  
**Goal:** Understand culture  
**Task:** Document CALMS  
**Concept:** Culture, Automation, Lean, Measurement, Sharing  
**Help:** More than just tools

**Exercise 592: Blameless Postmortem**  
**Goal:** Learn from failures  
**Task:** Write postmortem template  
**Concept:** Focus on improvement  
**Help:** What happened, why, prevention

**Exercise 593: SLI/SLO/SLA** ⭐  
**Goal:** Reliability metrics  
**Task:** Define for sample service  
**Concept:** Indicators, Objectives, Agreements  
**Help:** Measurable reliability

**Exercise 594: Change Management**  
**Goal:** Safe changes  
**Task:** Document change process  
**Concept:** Review, approve, rollback  
**Help:** Reduce risk

**Exercise 595: Documentation Practice** ⭐  
**Goal:** Write good docs  
**Task:** Document a system  
**Concept:** Runbooks, architecture  
**Help:** Others can maintain

**Exercise 596: Monitoring Dashboard** 📝  
**Goal:** Complete dashboard  
**Task:** Build Grafana dashboard  
**Concept:** Visualize system health  
**Help:** Key metrics visible

**Exercise 597: Complete CI/CD Pipeline** 📝  
**Goal:** End-to-end pipeline  
**Task:** Build, test, deploy  
**Concept:** Full automation  
**Help:** Commit to deployment

**Exercise 598: Infrastructure Project** 📝  
**Goal:** IaC complete setup  
**Task:** Ansible playbooks for full stack  
**Concept:** Reproducible infrastructure  
**Help:** Web server, database, monitoring

**Exercise 599: Container Platform** 📝  
**Goal:** Multi-service application  
**Task:** Docker Compose with multiple services  
**Concept:** Complete application stack  
**Help:** Frontend, backend, database, cache, monitoring

**Exercise 600: DevOps Portfolio** ⭐ 🎯 📝  
**Goal:** FINAL PROJECT  
**Task:** Build complete DevOps environment combining everything!  
**Components:**
- Git repository with branching strategy
- CI/CD pipeline (Jenkins/GitLab/GitHub Actions)
- Docker containers for application
- Docker Compose for local development
- Ansible playbooks for configuration
- Prometheus + Grafana monitoring
- Backup strategy implemented
- Security best practices applied
- Documentation for everything
**Concept:** Everything you've learned!  
**Help:** This is your DevOps showcase

---

## 📚 Learning Tips

### For Complete Beginners:
1. **Do exercises in order** - each builds on previous concepts
2. **Type every command** - don't copy/paste, muscle memory matters
3. **Read error messages** - Linux tells you what's wrong
4. **Take breaks** - 10-15 exercises per day is perfect
5. **Repeat difficult concepts** - marked with 🎯

### When Stuck:
1. Read the error message carefully
2. Check spelling and syntax
3. Google the exact error message
4. Use `man command` for help
5. Come back tomorrow with fresh eyes

### Marking Your Progress:
- Change ☐ to ✅ when complete
- Add 📝 when you're working on it
- Add 🎯 to exercises you want to practice more

### Study Schedule Suggestion:
- **Week 1-8:** Exercises 1-140 (Linux & Scripting)
- **Week 9-14:** Exercises 141-230 (System Admin & Networking)
- **Week 15-22:** Exercises 231-360 (Docker & Monitoring)
- **Week 23-30:** Exercises 361-480 (Git & CI/CD)
- **Week 31-38:** Exercises 481-540 (IaC)
- **Week 39-42:** Exercises 541-600 (Security & Projects)

---

## 🎯 Key Skills Summary

### Linux Fundamentals (Phase 1)
- Navigation: `cd`, `ls`, `pwd`
- Files: `cp`, `mv`, `rm`, `touch`, `mkdir`
- Viewing: `cat`, `less`, `head`, `tail`
- Finding: `find`, `grep`, `which`
- Permissions: `chmod`, `chown`
- Users: `whoami`, `sudo`, `su`

### Shell Scripting (Phase 2)
- Variables, conditions, loops
- Functions and arguments
- Text processing: `cut`, `awk`, `sed`
- Practical automation scripts

### System Administration (Phase 3)
- Package management: `apt`
- Services: `systemctl`
- Scheduling: `cron`
- Process management

### Networking (Phase 4)
- IP, DNS, routing
- SSH and secure access
- Firewall with UFW
- Network troubleshooting

### Docker (Phase 5)
- Containers and images
- Dockerfile creation
- Networking and volumes
- Docker Compose

### Monitoring (Phase 6)
- System monitoring tools
- Log management
- Prometheus metrics
- Grafana dashboards

### Git (Phase 7)
- Version control basics
- Branching and merging
- Remote repositories
- Collaboration workflows

### CI/CD (Phase 8)
- Pipeline concepts
- Jenkins, GitLab CI, GitHub Actions
- Automated testing and deployment

### Infrastructure as Code (Phase 9)
- Ansible for configuration
- Terraform for provisioning
- Modules and best practices

### Security (Phase 10)
- System hardening
- Container security
- Secrets management
- Backup and recovery

---

## 🎓 What Makes This Guide Effective?

1. **Zero to Hero** - Starts from absolute basics
2. **600 Exercises** - Comprehensive coverage
3. **Local Only** - No cloud accounts needed
4. **One Concept Each** - Digestible learning
5. **Practical Focus** - Real-world skills
6. **Progressive Difficulty** - Builds gradually
7. **Complete DevOps Path** - All major areas covered
8. **Hands-On** - Learn by doing
9. **Clear Structure** - 60 weeks of content
10. **Final Projects** - Apply everything learned

---

## 🚀 Next Steps After Completion

After finishing all 600 exercises, you should:

1. **Build a portfolio project** combining multiple skills
2. **Contribute to open source** DevOps tools
3. **Study for certifications** (CKA, AWS, etc.)
4. **Explore cloud platforms** (you now have the foundation)
5. **Learn Kubernetes** (natural next step after Docker)
6. **Practice interview questions** for DevOps roles
7. **Join DevOps communities** and share knowledge

Good luck on your DevOps journey! 🛠️








