# Object detection in urban environment
## 1. Selection of pre-trained [models](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md).
   This project use an object detection model with the Tensorflow Object Detection API and AWS Sagemaker.
   
| Pre-trained model from model zoo |
| ------------- | 
| EfficientDet D1 640x640  | 
| SSD MobileNet V2 FPNLite 640x640 |
| Faster R-CNN ResNet50 V1 640x640 |
## 2. Dataset
Front Camera Images from [Waymo Open Dataset](https://waymo.com/open/). Data are in TFRecord Format. 
## 3. Parameters of traning
| Setting | EfficientDet D1 | MobileNet V2 | Faster R-CNN ResNet50 V1 |
| ------------- | ------------- | ------------- |  ------------- | 
| num_ephocs: |  2000 | 2000 | 2000 |
| optimizer: |   momentum_optimizer | adam_optimizer | momentum_optimizer|      
| batch_size: | 8 | 8 | 8 |


## 4. Results

| Models | Results |
| ------------- | ------------- | 
| EfficientDet D1 640x64  | ![](media/output_efficientdet.gif) |
| SSD MobileNet V2 FPNLite 640x640 | ![](media/output_fasterresnet50.gif) |
| Faster R-CNN ResNet50 V1 640x640 | ![](media/output_mobilenet.gif) |

![](media/losses.png)
