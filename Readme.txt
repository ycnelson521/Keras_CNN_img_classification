This implemented a multi-layer convolution neural-network(CNN) to classiffy images.
The CNN is made of 4 CNN layers.
Layer configuration is (2,3,3)-(2,3,3)-(4,3,3)-(4,3,3)-8-label_cnt.
The training images of the same class should be basicly similar in view.
This CNN may be able to adapt to lightning variation and some outliers (non-scene objects).

No pretrained weight is prepared.
However, a new classification task with different images require addtional training or re-train.

To prepare the training data, put images of the same class into a directory under /train. (create it if it's not there)
To prepare the testing data, likewise, put images of the same class into a directory under /test. (create i if it's not there)
Modifying the path to training and testing directory enables running different training/testing.

The program will automatically traverse images in different class (label) directories.
All image will be loaded into memory.
Some computers may encounter “memory error" due to excessive memory usage.
(This should be modified for more efficient memory usage)
