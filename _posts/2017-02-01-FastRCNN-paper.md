---
layout: post
title: "Fast-RCNN-paper解析"
subtitle: Fast-R-CNN-paper解析
date: 2017-02-01 
author:    HY
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - Deep Learning
    - Object Detectiom
    - computer vision
    
---     


## Fast RCNN 论文
### 作者：Ross Girshick
### paper地址: [Fast R-CNN](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Girshick_Fast_R-CNN_ICCV_2015_paper.pdf)
#### 摘要
本文提出了一种快速的基于区域的卷积网络方法（fast R-CNN）用于目标检测。Fast R-CNN建立在以前使用的深卷积网络有效地分类目标的成果上。相比于之前的成果，Fast R-CNN采用了多项创新提高训练和测试速度来提高检测精度。Fast R-CNN训练非常深的VGG16网络比R-CNN快9倍，测试时间快213倍，并在PASCAL VOC上得到更高的精度。与SPPnet相比，fast R-CNN训练VGG16网络比他快3倍，测试速度快10倍，并且更准确。Fast R-CNN的Python和C ++（使用Caffe）实现以MIT开源许可证发布在：https://github.com/rbgirshick/fast-rcnn。
