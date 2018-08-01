---
layout: post
title: "R-FCN paper解析"
subtitle: "R-FCN paper解析"
date: 2017-05-1 
author:     HeYun
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - Deep Learning
    - Object Detectiom
    - computer vision
---     


# R-FCN 论文 
## 作者：Jifeng Dai, Yi Li, Kaiming He, Jian Sun
## paper地址: [R-FCN: Object Detection via Region-based Fully Convolutional Networks](https://arxiv.org/pdf/1605.06409.pdf)
### 摘要
我们提出了基于区域的全卷积网络，以实现准确和高效的目标检测。与先前的基于区域的检测器（如Fast/Faster R-CNN [6，18]）相比，这些检测器应用昂贵的每个区域子网络数百次，我们的基于区域的检测器是全卷积的，几乎所有计算都在整张图像上共享。为了实现这一目标，我们提出了位置敏感分数图，以解决图像分类中的平移不变性与目标检测中的平移变化之间的困境。因此，我们的方法可以自然地采用全卷积图像分类器的主干网络，如最新的残差网络（ResNets）[9]，用于目标检测。我们使用101层ResNet在PASCAL VOC数据集上展示了具有竞争力的结果（例如，2007数据集上83.6%的mAP）。同时，我们的测试结果是以每张图像170ms的测试速度实现的，比Faster R-CNN对应部分速度快2.5-20倍。代码公开发布在：[https://github.com/daijifeng001/r-fcn](https://github.com/daijifeng001/r-fcn）。
