# AlexNet
## Directory Structure
1. Golden C++
2. HLS
3. Python








## Golden C++

* conv.h - header file
* <layer>.cpp - C++ implementation of all individual layers in ALexNet
* top_testbench.cpp - wrapper testbench to call the layers serially as per the AlexNet architecture
* Makefile

### How to run

1. Just type make and ./csim.out. The C simulation will print expected and predicted class.

