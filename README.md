# YOLOv7 object detection counting blurring and croppring 

Download the pretrained YOLOv7 weights or you can use your own custom trained weights, and paste it in the folder "YOLOv7-object-detect-count-blur-crop" after clone the repository. 
- [Download](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt)


<img width="421" alt="image" src="https://user-images.githubusercontent.com/109053785/209044613-e6db91c5-1de7-475a-998e-55978ffd7f02.png">

## Installation

```
git clone https://github.com/Zeeshann1/YOLOv7-object-detect-count-blur-crop.git  # clone 
cd YOLOv7-object-detect-count-blur-crop
pip install -r requirements.txt  # install dependencies
```


## Detect & Blur Objects
```
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" --blurratio 20
```

## Detect & Blur Specific Class object
- Here we are blurrig class 0 that is person class.
```
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50
```

## Hide Detected Bounding Boxes
```
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50 --hidedetarea
```

## Detect & Crop Objects
```
python detect_and_crop.py --weights yolov7.pt --source "your video.mp4"
```

## Detect & Crop Specific Class Object
- Here we are cropping class 0 that is person class.
```
python detect_and_crop.py --weights yolov7.pt --source "your video.mp4" -classes 0
```
## Detect & Count Objects
```
!python detect_and_count.py --weights /content/yolov7/yolov7.pt --conf 0.1 --source /content/yolov7/inference/images
```
