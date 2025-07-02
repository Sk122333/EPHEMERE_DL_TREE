# Introduction

This github presents an active learning methodology combined with YOLOV11 in order to detect isolated tree from satellite images.

Thus, we can also define the notion of isolated tree which is a single tree or a small group of trees that stands apart from larger forested areas or continuous vegetation cover. Generally, these trees are often found in agricultural landscapes, urban areas, pastures, or open fields, where they are not connected to dense woodlands or forests. Those trees are indeed, by their spatial particularity, play a very important role and has a huge contribution to ecosystems service while being a sensitive indicator to a majority of biological variations.


## Installation

pip install -r requirements.txt

## Description

The first part consists from this three different inputs (Satellite image, a grid for dividing the satellite image into small images and a batch of trees) to create the following file structure :


![Image](https://github.com/user-attachments/assets/d815961a-3ceb-4c26-ba5d-ccd96e33d16b)



New_datas allow us just to store the images from the unlabeled dataset and in the txt file the score of mAP on the testset at the end of each iteration, the number and the name of the images which overcome the conditions of the detection before being injected in the trainset. 
Thus, the function SS_yolo.py and SS_yolo_function.py allow to train the semi-supervised model with YOLOv8.

## Output

You have in the folder Results, some examples of tree detection images predicted and their probability of distribution.


