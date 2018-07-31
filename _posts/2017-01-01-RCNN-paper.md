---
layout: post
title: RCNN-paper解析
subtitle: R-CNN-paper解析
date: 2017-01-01 
author:     HY
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - Deep Learning
    - Object Detectiom
    - computer vision
    
---     


# RCNN 论文
## 作者：Ross Girshick, Jeff Donahue, Trevor Darrell, Jitendra Malik
## paper地址: [Rich feature hierarchies for accurate object detection and semantic segmentation](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Girshick_Rich_Feature_Hierarchies_2014_CVPR_paper.pdf)
### 摘要
过去几年，在权威的PASCAL VOC数据集上，物体定位的性能已经达到一个稳定水平。表现最好的方法都是融合了多个低层次图像特征和高层次的上下文环境的复杂系统。本文提出一种简单的可扩展的检测算法，可以将VOC2012上期望平均精度的最好结果明显提升30%以上——达到了53.3%。我们的方法结合了两个关键因素：(1) 将大型卷积神经网络（CNNs）应用于自底向上区域推荐以定位和分割物体；（2）当标签训练数据不足时，先针对辅助任务进行有监督预训练，再进行特定任务的调优，就可以产生明显的性能提升。由于我们结合了区域推荐和CNNs，该方法被称为R-CNN：Regions with CNN features。我们对比了R-CNN和OverFeat，Overfeat是最近被提出的一个机遇类CNN架构的滑动窗口检测器，发现R-CNN在ILSVRC2013检测数据集上面的表现明显优于OverFeat。整个系统的源码在：https://people.eecs.berkeley.edu/~rbg/rcnn（新地址：https://github.com/rbgirshick/rcnn）
