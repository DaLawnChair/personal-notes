# YOLO (You Only Look Once)

Short YOLO history:
v1-v3: single state detections models with backbone-neck-head, works on different sizes thruugh mutli-scale branches
V4: uses Mish activation, PANet and data augmentations
V5: improves data augemtntation method and has mutliple versions
X: Multi-positive, ahnchor-free, and decoupeld head into the model
v6: repareamertization method to yolo, using EfficientREp Backbone and Rep-PAN neck
v7: implements E-ELAN for gradient paths improvement
V8: integrates all of them into a SOTA model


# Basics

Most models follow a Backbone, Neck, and Head architecture

Backbone:
* Feature extractor from the raw image (or augmented image) into features in accordance to multiple layers of the image
* Images are scaled down into a feature pyramid

Neck:
* feature fusion between each layer of the backbone

Head:
* outputs the classifier and the detections of the image

Pre-processing:
* augmentations to the image to make for feeding into the backbone
* Common ones:
	* Image rescaling
	* Intensity adjustments
	* Mixup
	* Moasic

Post processing:
* Lots of predictions from the head, most are bad or non-maximal
* Typically uses [[()() Non-Maximal Suppression (NMS)]] (all YOLO models except for 10 I believe)


### Choosing head size:
https://www.youtube.com/watch?v=U6rpkdVm21E&list=PLivJwLo9VCUJXdO8SiOjZTWr_fXrAy4OQ&index=5

Effectively you want the head of the model to contributed by the # input of the model you select.

ie if your input is `[1 512 13 13]`, and you want to classify 3 objects per cell inside of this 13x13 grid, you'd at least need 4 channels for positions of the box, 1 cell for probability of there being an object in the box, and num_classes for each probability of each class for that object.

Thus $\text{output from head to FC} = \text{num of objects per cell} \cdot (\text{bbox dimensions} +\text{1 channel for probability} + \text{num classes})$
