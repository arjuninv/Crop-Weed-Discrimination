# Crop-Weed-Discrimination Model | Tensorflow
A image classifier built with Tensorflow and Keras that uses a CNN to classify weeds and healthy crops.

## Why? 
India loses farm produce worth $11b to weeds every year. THis project aims to integrate with autonomous land drones that will propel itself across the fields and help descriminate between healthy crops and weeds, to take preventive measures like spraying pesticides.

## Model break down
Model: "sequential"
<div>
_________________________________________________________________<br>
Layer (type)                 Output Shape              Param #   <br>
=================================================================<br>
conv2d (Conv2D)              (None, 254, 254, 16)      448       <br>
_________________________________________________________________<br>
max_pooling2d (MaxPooling2D) (None, 127, 127, 16)      0         <br>
_________________________________________________________________<br>
conv2d_1 (Conv2D)            (None, 125, 125, 32)      4640      <br>
_________________________________________________________________<br>
max_pooling2d_1 (MaxPooling2 (None, 62, 62, 32)        0         <br>
_________________________________________________________________<br>
conv2d_2 (Conv2D)            (None, 60, 60, 32)        9248      <br>
_________________________________________________________________<br>
max_pooling2d_2 (MaxPooling2 (None, 30, 30, 32)        0         <br>
_________________________________________________________________<br>
flatten (Flatten)            (None, 28800)             0         <br>
_________________________________________________________________<br>
dense (Dense)                (None, 512)               14746112  <br>
_________________________________________________________________<br>
dense_1 (Dense)              (None, 1)                 513       <br>
=================================================================<br>
Total params: 14,760,961
Trainable params: 14,760,961
Non-trainable params: 0
_______________________
</div>


## Dataset 
- A collection of broad leaved dock images for weed sprayer: https://www.kaggle.com/gavinarmstrong/open-sprayer-images
- Training Set: 6027 Images
- Validation Set: 670 Images
