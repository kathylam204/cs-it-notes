# OS Security, Programming, and Administration

## OS Security, Programming, and Administration Commands/Terms
### Basic Commands:
- ls: List file names (like DOS dir).
- rmdir: Remove directory (only empty directories unless -R is used).
- who: List users currently logged in.
- touch: Change file timestamp (can create a blank file).
- date: Show current time and date.
- cat: Concatenate files and print to terminal.
- pwd: Print working directory.
- rm: Remove files.
- cd: Change directory.
- -p: Create missing directory parts (for mkdir).
- df: Show what disk holds a directory.
- grep: Search for a pattern in a file.
- mkdir: Make directory.

File System and Navigation
File Names and Pathnames:
Unix file names can contain any characters except /.
Absolute Pathname: Starts at the root (/).
Example: ls /usr/bin
Relative Pathname: Does not start at the root.
Example: ls unix/Syllabus
Special relative pathnames: . (current directory), .. (parent directory).

Commands:
ls: List files.
Options: -l (long format), -a (show hidden files), -F (show file types).
cd [directoryname]: Change directory.
Without parameter, it changes to home directory.
pwd: Print working directory.
df: Show disk holding a directory.

File Operations
Copying Files:
cp [options] source dest: Copy files.
Example: cp iamempty one/iammyownemptyfilename

Deleting Files:
rm [options] names: Remove files.

File Attributes:
Access Times: Creation, last change, last read.
Size, Owners, Permissions.

File Permissions:
r (read), w (write), x (execute).
ls -l: Shows file permissions.

Changing Permissions:
chmod mode file
Mode: [ugoa][+-=][rwx]
Example: chmod g-wx foo

Running and Managing Programs
Running a Program:
Type the program name with options.
Standard I/O: Input (keyboard), Output (screen), Error (screen).

Customization:
Shell customization via startup files (~/.bash_profile, ~/.bashrc).

Redirection:
>: Redirect output to a file.
Example: ls > lsout
<: Redirect input from a file.
Example: sort < nums
|: Pipe output of one command as input to another.
Example: ls | sort

Shell Scripting
Variables and Computation:
var=value: Assign value.
Access with $var.
Arithmetic: expr 5 + $i, or echo $[5+i].

Selection Constructs:
if statement
if <test>; then
	<statements>
[elif <test>; then
	<statements>]
[else
	<statements>]
fi

Repetition Constructs:
while loop:
while <test>; do
	<statements>
done
for loop:
for <var> in <list>; do
	<statements>
done

Additional Commands
Text Manipulation:
cut -d -f: Cut columns from a file.
Example: cut -d -f1,5 /etc/passwd | tail
echo: Print text to terminal.

Process Management:
&: Run a command in the background.
jobs: List running background jobs.
kill %<job_number>: Kill a background job.
ps: List processes.
kill -9 <pid>: Force kill a process.

Boot Process:
Stages: BIOS, Boot Loader, Kernel.
Commands: lsusb, systemctl.

Regular Expressions:
Literals: Exact characters to match.
Metacharacters: Special characters for patterns (^, *).
Escape Sequence: Use metacharacters as literals.
