# Segmentation_FCN
## Guide to get data
The dataset used in this project is PASCAL Visual Object Classes Challenge 2011 (known as VOC2011).
To download it and make the program work, frst you need to download the dataset in tar format.
```
$ curl -L http://host.robots.ox.ac.uk/pascal/VOC/voc2011/VOCtrainval_25-May-2011.tar \
> > VOCtrainval_25-May-2011.tar
```
Then extract it.
```
$ tar -xvzf VOCtrainval_25-May-2011.tar
```
Finally move the data to data folder.
```
$ mv TrainVal/VOCdevkit/VOC2011 /path/to/workspace/data
```
## Referred fles
The ```BilinearUpSampling.py``` and ```voc_generator.py``` are credit to keras-fcn by JihongJu (https://github.com/JihongJu/keras-fcn)

## Main files
### model.py
To build a FCN model based on VGG16.
### train.py
To train the model with VOC2011.
## Acknowledgements
Some of the codes are implemented from JihongJu’s work. These parameters and arguments save us a lot of
time to pick good initial values. We would like to express our warmest gratitude to Prof. Yao Wang, for her
instructive suggestions when we are confronted with problems of computing power. At the same time, we
are also grateful to Mr. Ish Kumar Jain for providing us with valuable advice and instructions concerning
Google Cloud Platform.
