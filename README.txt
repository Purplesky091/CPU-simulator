--ABOUT--
CPU simulator written in C++.
-Needed to run-
Must be ran through a Unix terminal as it uses the fork() function that
is exclusive to Unix versions of C++.

This is a project that simulates how a processor and memory communicate
with each other. The simulator can take in basic instructions and even
have interrupts occur. The amount of interrupts that will occur when a
program is run depends on the value specified by the user.

The project works by forking two processes. One process simulates what
Memory will do and one process simulates what the processor will do. The
two processes communicate through two pipes. One pipe is used for the
Memory process to send information to the processor process. The other
pipe is used for the processor to send information to the memory
process.

--HOW TO RUN--
Navigate to the folder containing the project files through the terminal
type "g++ *.cpp" to compile all files
type "./a.out "<text file name>" <timer value>

For example, if I wanted to run sample 2.txt with an interrupt value of
30, I would type
./a.out "sample 2.txt" 30
By default, the program will run "sample 2.txt"
