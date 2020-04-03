# Depth Map by Transfer Learning
A TensorFlow V2 implementation of _High Quality Monocular Depth Estimation via Transfer Learning_, [https://arxiv.org/abs/1812.11941](https://arxiv.org/abs/1812.11941).

## NN Architecture
DenseDepth uses an encoder-decoder architecture as shown in the figure. _[DenseNet169](https://arxiv.org/abs/1608.06993)_, pretrained for Image Classification on ImageNet, is used as encoder which converts input RGB image to feature vectors. Decoder consists of series of Upsampling layers which have skip-connections with the encoder. This model results in depth map at half the resolution of input image.

|![nn architecture](./img/archi.png) | ![nn model](./img/model.png)|
|--|--|
|Encoder-Decoder [1]|Layers [1]|

## Results
|![result](./img/result.png)|
|--|
|Results using a fraction of nyu depth dataset v2|

|![result](./img/loss.png)|
|--|
|Learning cruve|


## References
1. Ibraheem Alhashim and Peter Wonka, "High Quality Monocular Depth Estimation via Transfer Learning," 2018, [https://arxiv.org/abs/1812.11941](https://arxiv.org/abs/1812.11941)

2. [@ialhashim](https://github.com/ialhashim) - [DenseDepth](https://github.com/ialhashim/DenseDepth)

## Acknowledgements
Code borrows from [DenseDepth](https://github.com/ialhashim/DenseDepth).
