# AlexNet
## Directory Structure
1. Golden C++
2. HLS
3. Python

## HLS
This has all the unoptimized and optimised HLS directories for each individual layer along with the final AlexNet integration of all layers.
* Go to the directory you want to run
* Check the required txt files in testbench_\<layer\>.cpp
* Add required txt files 
* Just make and ./csim.out
* For vitis synthesis, just type _lastyear vitis_hls -f layer_synth.tcl_

## Python
* All data file (output, weights and bias) for each layer can be found in the **data_txt** directory.
* **epochs_50.ipynb** is the python code for our AlexNet architecture using tensorflow and keras. We referred to [1] for our python implementation.
* **Data_extract.ipynb** is the python code for extracting and storing each layer output, weights and bias into txt files.
* **epochs_50.h5** is our AlexNet model, which can directly be used for loading our implemented model.

[1] https://towardsdatascience.com/implementing-alexnet-cnn-architecture-using-tensorflow-2-0-and-keras-2113e090ad98

## Golden C++

* conv.h - header file
* <layer>.cpp - C++ implementation of all individual layers in ALexNet
* top_testbench.cpp - wrapper testbench to call the layers serially as per the AlexNet architecture
* Makefile

### How to run

1. Copy the input_conv1.txt, all weigths_\<layer\>.txt and all bias_\<layer\>.txt.
2. Just type make and type ./csim.out. The C simulation will print expected and predicted class.


