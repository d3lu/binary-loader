# Binary loader
Simplistic binary-loading interface agnostic of the underlying implementation, using major parts of libbfd functions and data structures. Inspired by the code in Practical Binary Analysis book.

## Usage
You have to run the compiled version of the loader along with an example executable file (e.g. /bin/ls) in order to get info about the sections and symbols of the executable.
```
./binary_loader /bin/ls
```
