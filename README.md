## README
---
**Object Detection Pipelines**

# TO DO

DETR
YOLOv5
EfficientDET
Faster RCNN
Image GPT - Open AI?
BERT


Notes on Object Detection: 

mAP Mean Average Precision 

Is the preferred metric for object detection. 

For each class the AP is calculated. The average precision is the area under the precision recall curve. The precision recall curve is created using the ordered list of object predictions (ordered based on confidence in the prediction).

When just looking at the first prediction, the precision is going to to be high (you're predicting just one object and as it's the object of highest confidence there's a good chance it's correct) but low recall, of all the objects present you're at most finding just one. AS you look at more and more predictions the precision will head down and the recall increase. (might be a bit zig zaggy)

The area under this curve is the average precision. 

The mean average precision is then just the mean for each of the classes. 

When you start calculating mAP you'll need to decide an IoU threshold. This is the threshold at which you allow a prediction of an object to be included as a correct object. So if you have a IoU threshold of 0.5 then the bounding boxes of the prediction and the actual will need to be less aligned than if you used a IoU of 0.9. You can draw precision recall curves for different IoUs. 

With mAP you can now compare the performance of different object detection algorithms and compare to the literature.

https://towardsdatascience.com/what-is-mean-average-precision-map-in-object-detection-8f893b48afd3



