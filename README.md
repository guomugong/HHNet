## Fundus Image Segmentation via Hierarchical Feature Learning
Please read my [paper](https://doi.org/10.1016/j.compbiomed.2021.104928) for more details!
### Introduction:
Fundus Image Segmentation (FIS) is an essential procedure for the automated diagnosis of ophthalmic diseases.  Recently, deep fully convolutional networks have been widely used for FIS with state-of-the-art performance. The representative deep model is the U-Net, which follows an encoder-decoder architecture. I believe it is suboptimal for FIS because consecutive pooling operations in the encoder lead to low-resolution representation and loss of detailed spatial information, which is particularly important for the segmentation of tiny vessels and lesions.  Motivated by this, a high-resolution hierarchical network (HHNet) is proposed to learn semantic-rich high-resolution representations and preserve spatial details simultaneously. Specifically, a High-resolution Feature Learning (HFL) module with increasing dilation rates was first designed to learn the high-level high-resolution representations. Then, the HHNet was constructed by incorporating three HFL modules and two feature aggregation modules. The HHNet runs in a coarse-to-fine manner, and fine segmentation maps are output at the last level. Extensive experiments were conducted on fundus lesion segmentation, vessel segmentation, and optic cup segmentation. The experimental results reveal that the proposed method shows highly competitive or even superior performance in terms of segmentation performance and computation cost, indicating its potential advantages in clinical application.

# Network Architecture
![image](https://github.com/guomugong/HHNet/blob/main/hhnet_arch.png)


## License
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)
[![Badge](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/#/zh_CN)
