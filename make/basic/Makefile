files := $(wildcard *.c)

# Important variables used by implicit rules
# CC: Program for compiling C programs; default cc
# CXX: Program for compiling C++ programs; default g++
# CFLAGS: Extra flags to give to the C compiler
# CXXFLAGS: Extra flags to give to the C++ compiler
# CPPFLAGS: Extra flags to give to the C preprocessor
# LDFLAGS: Extra flags to give to compilers when they are supposed to invoke the linker
CC = gcc 
CFLAGS = -g

all: file1.o

file1.o: file1.c

a := Hello World
hello: 
	echo $a
	printf '$a\n'

# Print out file information about every .c file
print: $(wildcard *.c)
	ls -la  $?

envs: first second
	# target name
	echo $@

	# Outputs all prerequisites newer than the target
	echo $?

	# Outputs all prerequisites
	echo $^

first second:
	touch $@

clean:
	rm file1.o first second