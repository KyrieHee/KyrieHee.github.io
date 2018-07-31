---
layout:     post
title:      Faster R-CNN-paper解析
subtitle:   Faster R-CNN-paper解析
date:       2017-03-01
author:     HY
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - Deep Learning
    - Object Detectiom
    
---

# Faster RCNN 论文
## 作者：Shaoqing Ren, Kaiming He, Ross Girshick, Jian Sun
## paper地址: [Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks](https://arxiv.org/abs/1506.01497.pdf)
### 摘要

目前最先进的目标检测网络需要先用区域建议算法推测目标位置，像SPPnet[7]和Fast R-CNN[5]这些网络已经减少了检测网络的运行时间，这时计算区域建议就成了瓶颈
问题。本文中，我们介绍一种区域建议网络（Region Proposal Network, RPN），它和检测网络共享全图的卷积特征，使得区域建议几乎不花时间。RPN是一个全卷积网
络，在每个位置同时预测目标边界和objectness得分。RPN是端到端训练的，生成高质量区域建议框，用于Fast R-CNN来检测。通过一种简单的交替运行优化方法，RPN和
Fast R-CNN可以在训练时共享卷积特征。对于非常深的VGG-16模型[19]，我们的检测系统在GPU上的帧率为5fps（包含所有步骤），在PASCAL VOC 2007和
PASCAL VOC 2012上实现了最高的目标检测准确率（2007是73.2%mAP，2012是70.4%mAP），每个图像用了300个建议框。代码已公开。
