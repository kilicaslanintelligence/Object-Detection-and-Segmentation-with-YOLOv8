# Object Detection and Segmentation with YOLOv8

## Installation
```
pip install ultralytics
```
### Object Detection in Photo
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source="img.jpg" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**
![img](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Image.webp)

**Object Detection Image**
![Object-Detection-Image](https://github.com/kilicaslanintelligence/Object-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Object-Detection-Image.webp)
___
### Object Segmentation in Photo
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='img.jpg' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('img.jpg', save=True)
```
**Example**

**Image**s
![img](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Image.webp)

**Object Segmentation Image**
![Object-Segmentation-Image](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Object-Segmentation-Image.webp)
___
### Object Detection in Video
#### CLI (Comman Line Interface)
```
yolo detect predict model=yolov8x.pt source="video.mp4" save=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Video.webp)](https://www.youtube.com/watch?v=wBG1KDi17QM)

Object Detection Video**
[![Object-Detection-Video](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Object-Detection-Video.webp)](https://www.youtube.com/watch?v=lvPSlkSZqyA)
___
### Object Segmentation in Video
#### CLI (Comman Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='video.mp4' save=true
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
results = model('video.mp4', save=True)
```
**Example**

**Video**
[![video](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Video.webp)](https://www.youtube.com/watch?v=wBG1KDi17QM)

**Object Segmentation Video**
[![Object-Segmentation-Video](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Object-Segmentation-Video.webp)](https://www.youtube.com/watch?v=psdXMi5fQ8U)
___
### Real Time Object Detection
#### CLI (Command Line Interface)
```
yolo detect predict model=yolov8x.pt source=0 show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Detection**
[![Real-Time-Object-Detection](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Detection-with-YOLOv8/Real-Time-Object-Detection.webp)](https://www.youtube.com/watch?v=yvONGbaFJ0g)
___
### Real Time Object Segmentation
#### CLI (Command Line Interface)
```
yolo task=segment mode=predict model=yolov8x-seg.pt source='0' show=True
```
#### Python
```
from ultralytics import YOLO

model = YOLO('yolov8x-seg.pt')
model.predict(source="0", show=True)
```
**Example**

**Real Time Object Segmentation**
[![Real-Time-Object-Segmentation](https://github.com/kilicaslanintelligence/Object-Detection-and-Segmentation-with-YOLOv8/blob/main/Object-Segmentation-with-YOLOv8/Real-Time-Object-Segmentation.webp)](https://www.youtube.com/watch?v=bhdDW9Fkcw0)