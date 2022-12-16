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
