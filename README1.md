###versions
#####CUDA:11.1
#####torch:1.7.1+cu110
#####torchvision:0.8.2+cu110

###Dataset
```
Annotations put in VOCdevkit/VOC2007
JPEGImages put in VOCdevkit/VOC2007


VOCdevkit  VOC2007 Annotations
                   ImageSets
                   JPEGImages
                   voc2yolo4.py
```
run
```
python3 voc_annotation.py
```
###train
```
python3 train.py
```
### pth model
#####yolov4-tiny
```
logs/yolov4-tiny/Epoch15-Total_Loss1.7743-Val_Loss2.6375.pth
```
#####RTSD-Net
```
logs/yolov4-cu-tiny-416/Epoch20-Total_Loss2.0437-Val_Loss2.7677.pth
```
###network
#####yolov4-tiny
```
nets/CSPdarknet53_tiny.py
```
#####RTSD-Net
```
nets/yu4_6_with_resblock_B.py
```
###predict
```
python3 predict.py
img/south0502-9-7.jpg
```
###FPS
```
python3 FPS_test.py
```
###pth is converted to onnx
```
python3 pth-onnx.py
```
###onnx model

#####yolov4-tiny
```
pth-onnx/yolov4-tiny-416.onnx
```
#####RTSD-Net
```
pth-onnx/yolov4-cu-tiny-416.onnx
```
###mAP
yolov3-tiny
```
map/yolov3-tiny/last/mAP.png
```
yolov4-tiny
```
map/yolov4-tiny/last/results/mAP.png
```
RTSD-Net
```
map/yu4_6_with_resblock_B/last/results/mAP.png
```
