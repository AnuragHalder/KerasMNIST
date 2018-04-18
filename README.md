# KerasMNIST

Inspired by Siraj Raval's video on YouTube about deploying your Keras model to production 

Had initial challenges in cloning and running the code, after researching made some updates to the `app_file.py`

To use your Keras model driven MNIST recoginition app on your local computer simply clone the directory:

`git clone https://github.com/AnuragHalder/KerasMNIST.git`

This will create a new directory for you `KerasMNIST`, please go into this directory and run the following command:

`python app_file.py` 

Here is a quick representation of the model used

Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 28, 28, 32)        320       
_________________________________________________________________
dropout_1 (Dropout)          (None, 28, 28, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 28, 28, 32)        9248      
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 14, 14, 32)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 14, 14, 64)        18496     
_________________________________________________________________
dropout_2 (Dropout)          (None, 14, 14, 64)        0         
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 14, 14, 64)        36928     
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 7, 7, 64)          0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 3136)              0         
_________________________________________________________________
dense_1 (Dense)              (None, 1024)              3212288   
_________________________________________________________________
dropout_3 (Dropout)          (None, 1024)              0         
_________________________________________________________________
dense_2 (Dense)              (None, 512)               524800    
_________________________________________________________________
dropout_4 (Dropout)          (None, 512)               0         
_________________________________________________________________
dense_3 (Dense)              (None, 10)                5130      
=================================================================
Total params: 3,807,210
Trainable params: 3,807,210
Non-trainable params: 0
_________________________________________________________________

Test_Accuracy:  0.9921
