## Introduction   
This repository contains a moded version of PyTorch YOLOv5 (https://github.com/ultralytics/yolov5). Which can be used easily in object detection and here I have trained model with only 300 epochs and below is the results.

<img src="https://github.com/Jaiminml/YOLOV5_CustomDataset/blob/master/runs/train/robo4_epoch150_s11/results.png" width="900">

## Requirements

Python 3.8 or later with all [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) dependencies installed, including `torch>=1.7`. To install run:
```bash
$ pip install -r requirements.txt
```


## Tutorials Reffered

* [Train Custom Data](https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data)&nbsp; 🚀 RECOMMENDED
* [Weights & Biases Logging](https://github.com/ultralytics/yolov5/issues/1289)&nbsp; 🌟 NEW
* [Multi-GPU Training](https://github.com/ultralytics/yolov5/issues/475)
* [PyTorch Hub](https://github.com/ultralytics/yolov5/issues/36)&nbsp; ⭐ NEW
* [ONNX and TorchScript Export](https://github.com/ultralytics/yolov5/issues/251)
* [Test-Time Augmentation (TTA)](https://github.com/ultralytics/yolov5/issues/303)
* [Model Ensembling](https://github.com/ultralytics/yolov5/issues/318)
* [Model Pruning/Sparsity](https://github.com/ultralytics/yolov5/issues/304)
* [Hyperparameter Evolution](https://github.com/ultralytics/yolov5/issues/607)
* [Transfer Learning with Frozen Layers](https://github.com/ultralytics/yolov5/issues/1314)&nbsp; ⭐ NEW
* [TensorRT Deployment](https://github.com/wang-xinyu/tensorrtx)



## Training

Trained with the batchsize of 16 and image size is reduced to 416, however, default size is 640. Also optimizer here used is adam.

!python train.py --img 416 --batch 16 --epochs 300 --data data.yaml --cfg yolov5s.yaml --weights ‘’ --name robo4_epoch150_s --adam

## Results

This model can predict if the mask is not weared properly. These are the results. 

<img src="https://github.com/Jaiminml/YOLOV5_CustomDataset/blob/master/runs/detect/exp22/image.jpg" width="900">
<img src="https://github.com/Jaiminml/YOLOV5_CustomDataset/blob/master/runs/detect/exp25/image3.jpg" width="900">


## Other information
For more detailed information about the algorithms and their corresponding lisences used in this project access their official github implementations.





