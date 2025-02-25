 Feature Pyramid Networks
https://www.youtube.com/watch?v=FKsgO0U7CUw
* Images can be scaled down in stages. Let input= \[1 3 416 416\]:
	* Low level : \[1 128 52 52\], for small detections
		* mainly captures spatial information
	* Mid level : \[1 256 26 26\], for medium detections
	* High level : \[1 512 13 13\], , for large detections
		* Now high level has the highest level of semantic information of the image and highest receptive fields, but is the least interpretable

Receptive fields:
* representation of a cell in a downsampled image to the original image
	* Ie a pixel from an image with 512 features will correspond to a large number of cells inside the original image

Feature Pyramid Networks (FNP) combines these levels into a single feature map for all stages, regardless of which level you are on

"A top down architecture with lateral connections is developed for building high-level semantic feature maps at all scales"

```python
hl_fm = torch.randn(size=(1, 512, 13, 13))
ml_fm = torch.randn(size=(1, 256, 26, 26))
torch.add(hl_fm, ml_fm)
# RuntimeError: The size of tensor a (13) must match the size of tensor b (26) at non-singleton dimension 3
```

Because these layers are different sizes, you can pass them through a convolutional layer with output 64 to get them all the same size, and then upsample the data, thus they should all have the same dimensionality.

```python
from functools import partial
from torchvision.ops.misc import Conv2dNormActivation

LeakyRelu_Inplace = partial(
    nn.LeakyReLU,
    negative_slope=0.1,
    inplace=True,
)
# get them to the same # of channels
ConvBlockReduceChannels = partial(Conv2dNormActivation, 
                                  kernel_size=1,
                                  activation_layer=LeakyRelu_Inplace)
# upsample
hl_upsampler = nn.Upsample(scale_factor=2, mode="nearest") 
```
Now upsampling is unwanted, so we can then define another convultional layer to compensate.
```python
ConvSmoother = partial(
                Conv2dNormActivation,
                  in_channels=64, 
                  out_channels=64, 
                  kernel_size=3, 
                  activation_layer=LeakyRelu_Inplace
               )

hl_ml_fused_smoother = ConvSmoother()

smooth_hl_ml_fused = hl_ml_fused_smoother(hl_ml_fused)
```
We do this for for all levels to get them to the same level, going top down.


Diagram of what is happening:
![[Pasted image 20250203202412.png]]

Questions:
* Can you use more conv blocks for extracting more features?
* Why decide on 64, why not 128 channels?
* Why not push from the other direction? ie push from low level to high level?


https://colab.research.google.com/drive/1sSlTMwEoCM7zE2_f7K36BDtFARGxugL2?usp=sharing#scrollTo=SBGSfzgo7El2 <- code implementations
