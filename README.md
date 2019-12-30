# CheXpert Dataset Classification

Stanford's CheXpert dataset (https://stanfordmlgroup.github.io/competitions/chexpert/) provides ~200K chest X-rays labelled with various conditions.  The goal of this project is to automate radiology for chest conditions.

Due to the dataset's size, I didn't include the data in the repo.  To run any of the notebooks, download the small dataset (lower resolution images) and place it in the repo's root directory.

## Strategy

The classification tree is hierarchical in nature (as seen in the image below).  The numbers on the chart correspond to the proportion of images in the dataset that present those conditions.  My strategy is to train reasonably good binary classifiers for the higher-level conditions then use those trained modules as building blocks for our multi-class classifiers, which will be submitted for evaluation.

![Condition hierarchy](https://stanfordmlgroup.github.io/competitions/chexpert/img/figure1.png)

## Results

Results for each iteration of the model can be found in their respective directory.

## Relevant Resources

### Classification
- LeNet-5 (The OG ConvNet): http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf
- AlexNet (ReLU Activation and Deeper Networks): https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf
- ZFNet: https://arxiv.org/pdf/1311.2901v3.pdf
- VGGNet: https://arxiv.org/pdf/1409.1556v6.pdf
- GoogleNet: https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Szegedy_Going_Deeper_With_2015_CVPR_paper.pdf
- ResNet: https://arxiv.org/pdf/1512.03385.pdf
- Wide ResNet: https://arxiv.org/pdf/1605.07146.pdf
- DenseNet: https://arxiv.org/pdf/1608.06993.pdf
- ResNeXt: https://arxiv.org/pdf/1605.07146.pdf
- Spatial Transformer Networks: https://arxiv.org/pdf/1506.02025.pdf
### Object Detection
- R-CNN: https://arxiv.org/pdf/1311.2524v5.pdf
- Fast R-CNN: https://arxiv.org/pdf/1504.08083.pdf
- Faster R-CNN: https://arxiv.org/pdf/1506.01497v3.pdf
### Improving Network Performance and Training Optimizations
- Batch Normalization: https://arxiv.org/pdf/1502.03167.pdf
- Dropout Regularization: https://machinelearningmastery.com/dropout-for-regularizing-deep-neural-networks/
