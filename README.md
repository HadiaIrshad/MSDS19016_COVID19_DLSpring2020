# MSDS19016_COVID19_DLSpring2020
This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes

# PART A:
In this part we classify data into normal and covid-19 by fine tuning different layers of vgg-16 and resnet-18 model.

## Data 
This dataset contains X-Ray images from 2 classes (Infected and Normal)
- Data can be downloaded from [here](https://drive.google.com/a/itu.edu.pk/uc?id=1-HQQciKYfwAO3oH7ci6zhg45DduvkpnK)

## Models
The fine tuned models can be found [here](https://drive.google.com/open?id=1NWe8Xu6RvqIXEmR1FtDu5BB4UQsUrCQa)

## Experiments

### VGG-16 
For VGG-16 best cores on test data s are as follows

<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/VGG16.JPG">
</p>

### RESNET-18
For Resnet-18 best cores on test data s are as follows

<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/resnet18.JPG">
</p>


# PART B:
In this part we classify data into covid-19 , pneumonia and normal by fine tuning vgg-16 and resnet-18 model.In this part Focal Loss is used to handle class imbalance

## Data:
This dataset contains X-Ray images from 3 classes (covid-19, pneumonia, normal)
- Data can be downloaded from [here](https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view?usp=sharing)

## Models
The fine tuned models can be found [here](https://drive.google.com/open?id=106ylwrwaaKHPFg4HqSkYlOc2SYjLncfI)

## Experiments:
It is multi label classification problem. The confusion matrixs and score for best model with and without focal loss are given below on validation data.

### Without Focal Loss
Vgg16 performed better then the resnet-18.
<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/vgg16_val_NFLa.JPG">
</p>
<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/vgg16_val_NFLb.JPG">
</p>

### With Focal Loss
Vgg16 performed better then the resnet-18 with focal loss.

<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/vgg16_val_FLa.JPG">
</p>
<p align="center">
  <img  src="https://github.com/HadiaIrshad/MSDS19016_COVID19_DLSpring2020/blob/master/images/vgg16_val_FLb.JPG">
</p>

