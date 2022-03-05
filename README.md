# simpleC
Python script that helps compile multiple **C/C++** files at **unix** environment using **gcc**. Developed for personal use.

## Installation
Cd to your C/C++ project directory, then

     curl https://raw.githubusercontent.com/tmin002/simpleC/main/sc.py > sc ; chmod a+x sc
## How to use

  1. You can type ./sc -h to get command usage.
  2. sc will generate output.bin as a compile result. (Sadly you cannot change its name)
  3. sc will create a folder named 'pwd' when executing output.bin using -r option. That folder will be the program's working directory.
  
## Examples

 Compile helloworld.c:

     ./sc helloworld.c

 Compile hellworld.c, helloworld.h and helloearth.c:

     ./sc  helloworld.c helloearth.c

 Compile helloworld.c and helloearth.c which are in the same folder named hello:

     ./sc hello

 Compile helloworld.c with its source code embedded:

     ./sc -d helloworld.c

 Compile helloworld.txt that has C code in it, and run output after compile:

     ./sc -sdr helloworld.txt
