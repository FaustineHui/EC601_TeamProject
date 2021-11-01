# EC601_TeamProject
A slide of introduction:
https://docs.google.com/presentation/d/1Ml08Yu5EcXgjh7OZnyqD4ar7gpJOCbgq9BWKe4Tht6Y/edit?usp=sharing

A slide of sprintf2:

https://docs.google.com/presentation/d/1rWxHLD39EQtXEbLIKtgPC7BiwJezJn6im4-S-1St2_0/edit?usp=sharing

## Project Name

 Building 3D scenes from 2D images using ML algorithms

## Problem Statement

* Introduction:

This topic involves converting 2D images into 3D models through machine learning. The main step of applying machine learning algorithms is in the part of constructing a depth map from a 2D image. I expect to use point clouds for processing. According to the traditional 2D to 3D conversion, the specific method is as follows,

Use the 2D image as the left view to estimate the depth map --> Convert image to point cloud --> Get the right view by rendering the point cloud --> Build a 3D picture or model

The public's demand for 3D images, movies, and videos is increasing day by day. However, direct 3D shooting is relatively cumbersome and costly, resulting in insufficient 3D resources actually generated to meet the needs of the public. In addition, games and the two-dimensional culture are prevailing at the moment, and people are very interested in the 3Dization of 2D characters.
This project will be able to generate 3D pictures, videos or models from 2D images. To meet the public's demand for 3D resources. The project will use machine learning algorithms to complete fully automatic conversion and try to ensure a good look and feel of the output results.

* Target Customer:

Two-dimensional culture lovers, individual users, 3D modeling workers

## Applications

Special effects movie production, Game modeling, Cultural relic restoration, 3D short video production

## Societal Significance of the Research

At present, many individual users have a particularly high demand for this technology. I personally think that this is based on the widespread dissemination of the virtual image of the two-dimensional culture. Many 2D characters and 2D images make people want to see them in 3D. This conversion technology can help them.
In addition, this conversion technology can also help film, animation, game and other industries to complete some simple tasks. Some 3D modeling that does not require absolute meticulousness can be completed quickly. Of course, some fine-grained work still cannot be replaced, but as the amount of data increases, this technology will also generate more and more refined results.

## 2D to 3D Video Conversion

* Abstract:

I choose this part as my main focus of interest, because there are many social needs in both aspects for individual pictures and continuous videos. Compared with image processing, video processing only adds frame extraction operations and finally continuous rendering.
I found that there are very few 2D to 3D conversions based on point cloud operations in the existing papers, but I still found some papers and operating methods that are useful for my project. Maybe it can help me do it better.

* An Improved Virtual Viewpoint Rendering Algorithm for Two Viewpoints:

This is a method proposed by others that can significantly improve the effect of the final synthesized 3D image. This method is based on the traditional DIBR algorithm, but adds a point of view. The required virtual viewpoints are synthesized through two viewpoints to generate the final 3D image.
Compared with the original algorithm, this improved algorithm will make the generated 3D images more authentic, that is, the look and feel is natural. I have used the DIBR algorithm and some simple 3D image conversion using this algorithm, and the output results are not satisfactory. The output 3D image still retains the characteristics of the 2D image.

<div align=center>
<img src="/images/fig1.gif" width="180" height="300" style="width:80%">
<div align=left>

* Improved Criminisi algorithm

In the problem of 3D image processing, blanks and stitching in the output image are common phenomena. Although there have been improved algorithms as above, it is found in research that there will still be cracks in the final generated image. So additional processing is necessary.
The repair algorithm can solve this problem well to effectively fill in the blank areas in the generated image.

<div align=center>
<img src="/images/fig2.gif" width="180" height="160" style="width:80%">
<div align=left>

* Conclusion

The processing method proposed by this research can optimize the output result to a large extent, and it is also an indispensable part of the project. But it does not involve the processing of point clouds. My research direction is mainly focused on completing the conversion through point clouds.

## Open Source Project

The open source project I mainly want to use is Pytorch3D. The goal of PyTorch3D is to help accelerate research in the intersection of deep learning and 3D. Many people have made considerable contributions to improving the processing speed. And the processing speed is also a point that must be achieved in my project. If the processing speed is too slow, it will be difficult to meet the needs of the public.
In addition, Pytorch3D provides a method of rendering color point clouds, which is also very important, which can greatly reduce the complexity of our post-processing. Pytorch3D has been quite mature in this regard, and based on the tolerance of BSD rules, it can be used directly.

## Reference

Z. Feng, Z. Chao, Y. Huamin and D. Yuying, "Research on Fully Automatic 2D to 3D Method Based on Deep Learning," 2019 IEEE 2nd International Conference on Automation, Electronics and Electrical Engineering (AUTEEE), 2019, pp. 538-541, doi: 10.1109/AUTEEE48671.2019.9033402.
