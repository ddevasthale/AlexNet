# AlexNet
## Directory Structure
1. Golden C++
2. HLS
3. Python

## HLS
* This has all the unoptimized and optimised HLS directory for each individual layer along with the final AlexNet integration of all layers.

## Python
* All data file (output, weights and bias) for each layer can be found in the **data_txt** directory.
* **epochs_50.ipynb** is the python code for our AlexNet architecture using tensorflow and keras.
* **Data_extract.ipynb** is the python code for extracting and storing each layer output, weights and bias into txt files.
* **epochs_50.h5** is our AlexNet model, which can directly be used for loading our implemented model.



## Golden C++

* conv.h - header file
* <layer>.cpp - C++ implementation of all individual layers in ALexNet
* top_testbench.cpp - wrapper testbench to call the layers serially as per the AlexNet architecture
* Makefile

### How to run

1. Copy the input_conv1.txt, all weigths_<layer>.txt and all bias_<layer>.txt.
2. Just type make and type ./csim.out. The C simulation will print expected and predicted class.


