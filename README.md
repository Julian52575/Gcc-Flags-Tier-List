## S Tier
### Summary
+ [Feature](#feature-section)
  + [-I](#-i)
+ [Debug](#debugging-section)
  + [-g](#-g)
  + [-wall](#-wall)
  + [-wextra](#-wextra)
     
###### Remember the work / usage / reasoning format Julian !
# Feature Section
### All the flags found here are required to access some of the C language feature which explain their overall usefulness, and therefore, #1 on the list.

## -I 
### Reasoning : Clean C code *needs* the use of headers
#### -I _directory_ specify the _directory_ to search for your[^OSheader] header files. Header files are commonly used for prototyping your function to avoid interpreting every return type as an int, including other header files and creating structures. Any self-respecting C coder use headers.

## -L 
### Reasoning : WiP
#### -L _library file_ .
    
# Debugging Section
### The folowing flags are used for debugging a source code, they might have some drawback but they are super helpful to so many developers out there. You could theoretically make do without it, but you would be taking huge risks and wasting a lot of time.
### Warning flags are placed higher that debug flags such as -g, due to being the 1st -Wall ~(got it ?)~ against crashes and bugs.


## -Wall
### Reasoning : Warning are too important and -Wall acts on behalf of so many warning enabler flags
#### -Wall acts like *52* different warning flags[^ManPage] to notice you on every mistake the compiler finds. When you are programming something, especially in a lower level language such as C or C++, you need to be rigourous on everything you do.

## -Wextra
### Reasoning : Warning are too important and -Wall acts on behalf of some warning enabler flags
#### Only 17 flags this time, for smaller and rarer mistake you might make. Still very useful.

## -g
### Reasoning : Debug symbols are a must for quickly debugging a program
#### -g Enable debugging symbols to be added inside the binary during the compilation, which allows a debugger like _`gdb`_ or _`valgrind`_ to report the source code file, function and line the error happened. However, it should be noted that having debugging symbols leads to heavier binary and is an open door to Reverse Engineering...




##### You are free and encouraged to give your feedback under the 5th ammendment by creating an Issue on the relevant branch, let's _```make```_ this the ultimate collaborative tier list ! Have a good read !




















[^OSheader]: Glibc / OS header files should be precised with _-isystem_ 
[^ManPage]: According to https://man7.org/linux/man-pages/man1/gcc.1.html
