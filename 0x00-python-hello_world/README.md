Task 0 Write a Shell script that runs a Python script.

The Python file name will be saved in the environment variable $PYFILE step 1: create your main.py file step 2: create your 0-run file and make it executable

Task 1 Write a Shell script that runs Python code.

The Python code will be saved in the environment variable $PYCODE

guillaume@ubuntu:/py/0x00$ export PYCODE='print(f"Best School: {88+10}")' guillaume@ubuntu:/py/0x00$ ./1-run_inline Best School: 98 guillaume@ubuntu:~/py/0x00$

Task 2 Write a Python script that prints exactly "Programming is like building a multilingual puzzle, followed by a new line.

Use the function print
guillaume@ubuntu:/py/0x00$ ./2-print.py "Programming is like building a multilingual puzzle guillaume@ubuntu:/py/0x00$

Print integer mandatory
Complete this source code in order to print the integer stored in the variable number, followed by Battery street, followed by a new line.

You can find the source code here
The output of the script should be:
    the number, followed by Battery street,
    followed by a new line
You are not allowed to cast the variable number into a string
Your code must be 3 lines long
You have to use f-strings tips
guillaume@ubuntu:/py/0x00$ ./3-print_number.py 98 Battery street guillaume@ubuntu:/py/0x00$

Print float mandatory
Complete the source code in order to print the float stored in the variable number with a precision of 2 digits.

You can find the source code here
The output of the program should be:
    Float:, followed by the float with only 2 digits
    followed by a new line
You are not allowed to cast number to string
You have to use f-strings
guillaume@ubuntu:/py/0x00$ ./4-print_float.py Float: 3.14 guillaume@ubuntu:/py/0x00$

Print string mandatory
Complete this source code in order to print 3 times a string stored in the variable str, followed by its first 9 characters.

You can find the source code here
The output of the program should be:
    3 times the value of str
    followed by a new line
    followed by the 9 first characters of str
    followed by a new line
You are not allowed to use any loops or conditional statement
Your program should be maximum 5 lines long
guillaume@ubuntu:/py/0x00$ ./5-print_string.py Holberton SchoolHolberton SchoolHolberton School Holberton guillaume@ubuntu:/py/0x00$

Play with strings mandatory
Complete this source code to print Welcome to Holberton School!

You can find the source code here
You are not allowed to use any loops or conditional statements.
You have to use the variables str1 and str2 in your new line of code
Your program should be exactly 5 lines long
guillaume@ubuntu:/py/0x00$ ./6-concat.py Welcome to Holberton School! guillaume@ubuntu:/py/0x00$ wc -l 6-concat.py 5 6-concat.py guillaume@ubuntu:~/py/0x00$

Copy - Cut - Paste mandatory
Complete this source code

You can find the source code here
You are not allowed to use any loops or conditional statements
Your program should be exactly 8 lines long
word_first_3 should contain the first 3 letters of the variable word
word_last_2 should contain the last 2 letters of the variable word
middle_word should contain the value of the variable word without the first and last letters
guillaume@ubuntu:/py/0x00$ ./7-edges.py First 3 letters: Hol Last 2 letters: on Middle word: olberto guillaume@ubuntu:/py/0x00$ wc -l 7-edges.py 8 7-edges.py

Create a new sentence mandatory
Complete this source code to print object-oriented programming with Python, followed by a new line.

You can find the source code here
You are not allowed to use any loops or conditional statements
Your program should be exactly 5 lines long
You are not allowed to create new variables
You are not allowed to use string literals
guillaume@ubuntu:/py/0x00$ ./8-concat_edges.py object-oriented programming with Python guillaume@ubuntu:/py/0x00$ wc -l 8-concat_edges.py 5 8-concat_edges.py guillaume@ubuntu:~/py/0x00$

Easter Egg mandatory
Write a Python script that prints “The Zen of Python”, by TimPeters, followed by a new line.

Your script should be maximum 98 characters long (please check with wc -m 9-easter_egg.py)
Linked list cycle mandatory
Technical interview preparation:

You are not allowed to google anything
Whiteboard first
This task and all future technical interview prep tasks will include checks for the efficiency of your solution, i.e. is your solution’s runtime fast enough, does your solution require extra memory usage / mallocs, etc.
Write a function in C that checks if a singly linked list has a cycle in it.

Prototype: int check_cycle(listint_t *list);
Return: 0 if there is no cycle, 1 if there is a cycle
Requirements:

Only these functions are allowed: write, printf, putchar, puts, malloc, free
Hello, write #advanced
Write a Python script that prints exactly and that piece of art is useful - Dora Korpar, 2015-10-19, followed by a new line.

Use the function write from the sys module
You are not allowed to use print
Your script should print to stderr
Your script should exit with the status code 1
guillaume@ubuntu:/py/0x00$ ./100-write.py and that piece of art is useful - Dora Korpar, 2015-10-19 guillaume@ubuntu:/py/0x00$ echo $? 1 guillaume@ubuntu:/py/0x00$ ./100-write.py 2> q guillaume@ubuntu:/py/0x00$ cat q and that piece of art is useful - Dora Korpar, 2015-10-19 guillaume@ubuntu:~/py/0x00$

Compile #advanced
Write a script that compiles a Python script file.

The Python file name will be stored in the environment variable $PYFILE

The output filename has to be $PYFILEc (ex: export PYFILE=my_main.py => output filename: my_main.pyc)

guillaume@ubuntu:~/py/0x00$ cat main.py #!/usr/bin/python3 print("Best School")

guillaume@ubuntu:/py/0x00$ export PYFILE=main.py guillaume@ubuntu:/py/0x00$ ./101-compile Compiling main.py ... guillaume@ubuntu:/py/0x00$ ls 101-compile main.py main.pyc guillaume@ubuntu:/py/0x00$ cat main.pyc | zgrep -c "Best School" 1 guillaume@ubuntu:/py/0x00$ od -t x1 main.pyc # SYSTEM DEPENDANT => CAN BE DIFFERENT 0000000 ee 0c 0d 0a 91 26 3e 58 31 00 00 00 e3 00 00 00 0000020 00 00 00 00 00 00 00 00 00 02 00 00 00 40 00 00 0000040 00 73 0e 00 00 00 65 00 00 64 00 00 83 01 00 01 0000060 64 01 00 53 29 02 7a 10 48 6f 6c 62 65 72 74 6f 0000100 6e 20 53 63 68 6f 6f 6c 4e 29 01 da 05 70 72 69 0000120 6e 74 a9 00 72 02 00 00 00 72 02 00 00 00 fa 07 0000140 6d 61 69 6e 2e 70 79 da 08 3c 6d 6f 64 75 6c 65 0000160 3e 02 00 00 00 73 00 00 00 00 0000172 guillaume@ubuntu:/py/0x00$

ByteCode -> Python #1 #advanced
Write the Python function def magic_calculation(a, b): that does exactly the same as the following Python bytecode:

3 0 LOAD_CONST 1 (98) 3 LOAD_FAST 0 (a) 6 LOAD_FAST 1 (b) 9 BINARY_POWER 10 BINARY_ADD 11 RETURN_VALUE

