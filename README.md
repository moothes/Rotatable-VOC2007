# PASCAL-VOC2007
Annotate images by some points. This policy makes the image rotatable in detection.

It took me 10 hours every day in 2 weeks to annotate all images. 
By the way, some annotation errors in the original VOC2007 dataset are fixed in our annotations.
For a fair comparison, I only annotate the objects that are annotated in the original dataset.

We test the new annotations using SSD, which causes a 0.3 mAP drop in original images.
However, if we rotate the images by 75 degrees, the mAP of SSD that train on original datasets drop to 20.0+, while the network that trained on our new data remains 40.0+ mAP.  
