
# FrRCNN + DeepSort

For assignment reasons I have to modify the yolov5's inference codes and instead of using yolov5 model I use Faster RCNN model from pytorch.

The codes specifically for football-video.mp4 because I ignore all COCO labels except person and sports ball, but you can fit your own labels.



## References

This directory mainly follows codes from the article [Understanding Multiple Object Tracking using DeepSORT](https://learnopencv.com/understanding-multiple-object-tracking-using-deepsort/)

And using codes from these Projects:

 - [yolov5](https://github.com/ultralytics/yolov5)
 - [deepsort](https://github.com/nwojke/deep_sort)
 - [Understanding Multiple Object Tracking using DeepSORT](https://github.com/spmallick/learnopencv/tree/master/Understanding-Multiple-Object-Tracking-using-DeepSORT)

 


## Running football test

Firstly clone this repository

```bash
  git clone https://github.com/matthewwang16czap/yolov5_frrcnn_deepsort.git
```

go to yolov5 directory

```bash
  cd yolov5_frrcnn_deepsort/yolov5
```

run

```bash
python frrcnn_track.py --img 640 --source ./football-video.mp4 --save-txt --classes 0 32 --line-thickness 1
```

the result is stored in /runs

    
