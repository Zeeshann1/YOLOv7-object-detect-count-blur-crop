Download the pretrained YOLOv7 weights or you can use your own custom trained weights, and paste it in the folder "YOLOv7-object-detect-count-blur-crop"
Download Link: https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt
<img width="421" alt="image" src="https://user-images.githubusercontent.com/109053785/209044613-e6db91c5-1de7-475a-998e-55978ffd7f02.png">

# YOLOv7_object_detect_count_blur_crop


#if you want to change source file
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" --blurratio 20

#for specific class (person)
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50

#hide-detected-bounding-boxes
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50 --hidedetarea





#if you want to change source file
python detect_and_crop.py --weights yolov7.pt --source "your video.mp4"

#for specific class (person)
python detect_and_crop.py --weights yolov7.pt --source "your video.mp4" -classes 0



!python detect_and_count.py --weights /content/yolov7/yolov7.pt --conf 0.1 --source /content/yolov7/inference/images
