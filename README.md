# seals_deep_learning_video_classification

This repository contains all code related to research into streaming video classification and object detection for the particular application of detecting seals in underwater video streams from the back of boats out at sea. 

## Researchers:
* Dr. Ian Durbach (UCT, AIMS)
* Alex Conway (UCT, NumberBoost)

## Progress 
Models:
* [x] CNN: VGG
* [x] CNN: ResNet
* [X] CNN: XCeption
* [ ] OBJ DETECTION: FR-CNN
* [ ] OBJ DETECTION: YOLO V4
* [ ] OBJ DETECTION: Facebook Detectron Lib Algos
* [ ] VIDEO: LSTM on top of CNN frames
* [ ] VIDEO: CNN on top of CNN frames
* [ ] CNN: Ensemble
* [ ] META: Ensembled CNN model applied to detected object regions from best OBJ detection model

If we have time (lol):
* [ ] Reinforcement learning model

Improvements to try:
* [ ] Image data augmentation (flip and rotate and add noise)
* [ ] Video data augmentation
* [ ] Train attentional model

We anticipate:
1. LSTM on top of sequence of frames will outperform treating the frames as independent then applying a filter to the results
2. Ensemble CNN model should outperform
3. Ensembled video model should outperform
4. Adding data augmentations should improve performance

## Setup

The model was trained on an aws `p2.xlarge` instance with the nvidia deep learning ami`.

The anaconda 3 python distribution was used with the latest versions of all dependencies as at 01/05/2018. 

Just `pip install lib_name_here` for anything not already installed.

To start, just run `jupyter notebook` in this folder that contains the README and `notebooks` folder.
