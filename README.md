# Image_colorization
Convolutional Neural Network that converts black and white image to coloured image

## OVERVIEW
This code is an implementation of the mentioned [research paper](http://iizuka.cs.tsukuba.ac.jp/projects/colorization/data/colorization_sig2016.pdf) in pytorch.
This paper presents a novel technique to automatically colorize grayscale images that combines both global priors and local image features.
Based on Convolutional Neural Networks,this deep network features a fusion layer that allows the model to elegantly merge local information dependent on small image patches with global priors computed using the entire image.
The network learns both local features and global features jointly in a single framework which can then be used on images of any resolution.

Moreover,we optimized the code so that it can be trained using transfer learning.

## REQUIREMENTS
    -Pytorch
    -OS
    -opencv
    -numpy

## ARCHITECTURE
#### This model consists of four main components:
    1)low-level features network
    2)mid-level features network
    3)global features network
    4)colorization network
    
![alt text](https://github.com/25abhishek/Image_colorization/blob/master/Images/model.png)

The components are all tightly coupled and trained in an end-to-end fashion.
The output of this model is the chrominance of the image which is fused with the luminance to form the output image.

For further details,please check the [research paper](http://iizuka.cs.tsukuba.ac.jp/projects/colorization/data/colorization_sig2016.pdf).

## RESULTS

![alt text](https://github.com/25abhishek/Image_colorization/blob/master/Images/result.png)
