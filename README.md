# Codes-for-Lane-Detection
Codes for the CNN-based lane detection models. (expected release date: 2018.11.20)

### Timeline
I will release the torch code in 2018.11.20. Tensorflow and pytorch version of the model will be released thereafter.

### Prerequisites
- [Torch](http://torch.ch/docs/getting-started.html)
- [Tensorflow](https://www.tensorflow.org/)
- [Pytorch](https://pytorch.org/)

### Tensorflow version of SCNN

Progress:
- [ ] Define network architecture (VGG-16 (done) + message passing)
- [x] Load pre-trained weights
- [ ] Define dataloader (load images and labels (done) + data augmentation)
- [ ] Testing (generate probability maps + smoothing)
- [ ] Training (cross entropy loss and sigmoid loss (done) + validation)
- [ ] using multiple GPUs
- [ ] clean the code and make them reproducible

### Pytorch version of SCNN

Progress:
- [ ] Define network architecture (VGG-16 + message passing)
- [ ] Load pre-trained weights
- [ ] Define dataloader (load images and labels + data augmentation)
- [ ] Testing (generate probability maps + smoothing)
- [ ] Training (cross entropy loss and sigmoid loss + validation)
- [ ] using multiple GPUs
- [ ] clean the code and make them reproducible

### Cite our paper
Our paper working on lane detection will be available soon!

### Acknowledgement
This repo is built upon [SCNN](https://github.com/XingangPan/SCNN) and [LaneNet](https://github.com/MaybeShewill-CV/lanenet-lane-detection)

### Contact
If you have any problems in reproducing the results, just raise an issue in this repo.
