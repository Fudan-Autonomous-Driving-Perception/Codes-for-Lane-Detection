Codes for CNN-based lane detection models.

# Timeline

- [SCNN-Tensorflow](./SCNN-Tensorflow) is released. (2018-11-24)

# Content

* [Prerequisites](#Prerequisites)
* [Models](#Models)
  * [SCNN-Tensorflow](#SCNN-Tensorflow)
  * [SCNN-Pytorch](#SCNN-Pytorch)
  * [Our-Model](#Our-Model)
* [Datasets](#Datasets)
  * [TuSimple](#TuSimple)
  * [CULane](#CULane)
  * [BDD100K](#BDD100K)
* [Others](#Others)
  * [Citation](#Citation)
  * [Acknowledgement](#Acknowledgement)
  * [Contact](#Contact)

# Prerequisites
- [Torch](http://torch.ch/docs/getting-started.html)
- [Tensorflow](https://www.tensorflow.org/)
- [Pytorch](https://pytorch.org/)

# Models

Preliminary results on CULane testing set (F1-measure, waiting for updates):

|Category|[SCNN-Torch](https://arxiv.org/pdf/1712.06080.pdf)|SCNN-Tensorflow (old)|SCNN-Pytorch|
|:---:|:---:|:---:|:---:|
|Normal|90.6|80.0|--|
|Crowded|69.7|57.1|--|
|Night|66.1|50.8|--|
|No line|43.4|35.0|--|
|Shadow|66.9|45.6|--|
|Arrow|84.1|68.3|--|
|Dazzle light|58.5|48.7|--|
|Curve|64.4|51.6|--|
|Crossroad|1990|4480|--|
|Total|71.6|58.7|--|

## SCNN-Tensorflow

Update:

Testing the performance now.

Notes:

Please go to [SCNN-Tensorflow](./SCNN-Tensorflow) to see detailed instructions. 

## SCNN-Pytorch

Progress (on-going):
- [ ] Define network architecture (VGG-16 + message passing)
- [ ] Load pre-trained weights
- [ ] Define dataloader (load images and labels + data augmentation)
- [ ] Testing (generate probability maps + smoothing)
- [ ] Training
- [ ] validation
- [ ] using multiple GPUs
- [ ] clean the codes and make them reproducible

## Our-Model

Coming soon.

# Datasets

## TuSimple

The ground-truth labels of TuSimple testing set is now available at [TuSimple](https://github.com/TuSimple/tusimple-benchmark/issues/3). Please evaluate your pred.json using the labels and [this script](https://github.com/TuSimple/tusimple-benchmark/blob/master/evaluate/lane.py).

## CULane

The whole dataset is available at [CULane](https://xingangpan.github.io/projects/CULane.html).

## BDD100K

The whole dataset is available at [BDD100K](http://bdd-data.berkeley.edu/).

# Others

## Citation

If you use the codes, please cite the following publications:

``` 
@inproceedings{pan2018SCNN,  
  author = {Xingang Pan, Jianping Shi, Ping Luo, Xiaogang Wang, and Xiaoou Tang},  
  title = {Spatial As Deep: Spatial CNN for Traffic Scene Understanding},  
  booktitle = {AAAI Conference on Artificial Intelligence (AAAI)},  
  month = {February},  
  year = {2018}  
}
```
Our paper working on lane detection will be available soon!

## Acknowledgement
This repo is built upon [SCNN](https://github.com/XingangPan/SCNN) and [LaneNet](https://github.com/MaybeShewill-CV/lanenet-lane-detection)

## Contact
If you have any problems in reproducing the results, just raise an issue in this repo.
