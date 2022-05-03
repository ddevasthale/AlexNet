# AlexNet
## Directory Structure
1. Golden C++
2. HLS
3. Python

## HLS
This has all the unoptimized and optimised HLS directories for each individual layer along with the final AlexNet integration of all layers.
* Go to the directory you want to run
* Add required txt files
* Just make and ./csim.out
* For vitis synthesis, just type lastyear vitis_hls -f layer_synth.tch

## Python
* All data file (output, weights and bias) for each layer can be found in the **data_txt** directory.
* **epochs_50.ipynb** is the python code for our AlexNet architecture using tensorflow and keras. [1] This is the python model we referred to for our implementation.
* **Data_extract.ipynb** is the python code for extracting and storing each layer output, weights and bias into txt files.
* **epochs_50.h5** is our AlexNet model, which can directly be used for loading our implemented model.

[1] https://towardsdatascience.com/implementing-alexnet-cnn-architecture-using-tensorflow-2-0-and-keras-2113e090ad98
