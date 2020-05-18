# Binary loader
Simplistic binary-loading tool agnostic of the underlying implementation, using major parts of libbfd functions and data structures while it doesn't expose any of them. Inspired by the code in Practical Binary Analysis book. For simplicity, the interface is kept as basic as possible, exposing only those parts of the binary that are needed.


## Compilation
First, you have to compile / build the final version of this tool with a g++ command linking the libbfd like this :
```
g++ binary_loader.cc loader_print.cc -o binary_loader -lbfd
```


## Usage
You have to run the compiled version of the loader along with an example executable file (e.g. /bin/ls) in order to get info about the sections and symbols of the executable.
```
./binary_loader /bin/ls
```

![image](https://github.com/d3lu/binary-loader/blob/master/loader.png?raw=true "Usage of binary loader")
