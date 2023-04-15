This directory mainly follows codes from the article [Understanding Multiple Object Tracking using DeepSORT](https://learnopencv.com/understanding-multiple-object-tracking-using-deepsort/)

For assignment reasons I have to modify the yolov5's inference codes and instead of using yolov5 model I use Faster RCNN model from pytorch.

The codes specifically for football-video.mp4 because I ignore all COCO labels except person and sports ball, but you can fit your own labels.

to run:

python frrcnn_track.py  --img 640  --source ./football-video.mp4 --save-txt --classes 0 32 --line-thickness 1

results are saved in /Runs

