# Surface Defect Detection: Dataset & Papers <sup>📌</sup>
<a href="https://github.com/Luckycat518"><img src="https://img.shields.io/badge/GitHub-@Luckycat518-000000.svg?logo=GitHub" alt="GitHub" target="_blank"></a>
<a href="https://charmve.github.io/computer-vision-in-action/" target="_blank"><img src="https://img.shields.io/badge/Computer Vision-000000.svg?logo=GitBook" alt="Computer Vision in Action"></a>
[![License](https://img.shields.io/github/license/Charmve/Surface-Defect-Detection)](LICENSE)

# Table of Contents

- [Introduction](#introduction)
- [Key Issues](#1-key-issues-in-surface-defect-detection)
  - [Small Sample Problem](#1small-sample-problem)
  - [Real-time Problem](#2real-time-problem)
- [Our Dataset](#2-our-dataset-for-industrial-surface-defect-detection)
  - [Steel Surface: NEU-CLS](#1steel-surface-neu-cls)
- [Papers](#4-surface-defect-detection-papers)
- [Acknowledgements](#acknowledgements)
- [Download](#download)
- [Notification](#notification)
- [Citation](#-citation)


## Introduction

<p>At present, surface defectxxxx.</p>

<p>Compared with the clear classification, detection and segmentation tasks in computer vision, the requirements for defect detection are very general. In fact, its requirements can be divided into three different levels: "what is the defect" (<strong>classification</strong>), "where is the defect" (<strong>positioning</strong>) and "How many defects are" (<strong>split</strong>).</p>



## 1. Key Issues in Surface Defect Detection

### 1）Small Sample Problem

<p>The current deep xxxxx.</p>

<p>xxxxx<b>small sample problem</b>xxx:</p>


<b>- Data Amplification and Generation</b>
<p> The most commonly used defect image expansion method is to use multiple image processing operations such as mirroring, rotation, translation, distortion, filtering, and contrast adjustment on the original defect samples to obtain more samples. Another more common method is data synthesis, where individual defects are often fused and superimposed on normal (non-defective) samples to form defective samples.</p>

<b>- Network Pre-training and Transfer Learning</b>
<p>Generally speaking, using small samples to train deep learning networks can easily lead to <strong>overfitting</strong>, so methods based on pre-training networks or transfer learning are currently one of the most commonly used methods for samples.</p>


<b>- Reasonable Network Structure Design</b>
<p>The need for samples can also be greatly reduced by designing a reasonable network structure. Based on the compressed sampling theorem to compress and expand small sample data, we use CNN to directly classify the compressed sampling data features. Compared with the original image input, compressing the input can greatly reduce the network's demand for samples. In addition, the surface defect detection method based on the twin network can also be regarded as a special network design, which can greatly reduce the sample requirement.</p>


<b>- Unsupervised or Semi-supervised Method</b>

In the unsupervised model, only normal samples are used for training, so there is no need for defective samples. The semi-supervised method can use unlabeled samples to solve the network training problem in the case of small samples.

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

### 2）Real-time Problem

<p>The defect detection methods based on deep learning include three main links in industrial applications: <b>data annotation</b>, <b>model training</b>, and <b>model inference</b>. Real-time in actual industrial applications pays more attention to model inference. At present, most defect detection methods are concentrated in the accuracy of classification or recognition, little attention is paid to the efficiency of model inference. There are many methods for accelerating the model, such as model weighting and model pruning. In addition, although the existing deep learning model uses GPU as a general-purpose computing unit(GPGPU), with the development of technology, it is believed that FPGA will become an attractive alternative.</p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## 2. Our dataset for Industrial Surface Defect Detection

### 1）Steel Surface: NEU-CLS

NEU-CLS can be used for classification and positioning tasks.

- :x: Official Link：http://faculty.neu.edu.cn/yunhyan/NEU_surface_defect_database.html 

<b> latest access 🔗  - ([#16](https://github.com/Charmve/Surface-Defect-Detection/issues/16)) </b>

<div align=center><img src="https://img-blog.csdnimg.cn/20200927223042720.png"></div>

<p>The surface defect dataset released by Northeastern University (NEU) collects six typical surface defects of hot-rolled steel strips, namely rolling scale (RS), plaque (Pa), cracking (Cr), pitting surface (PS), inclusions (In) and scratches (Sc). The dataset includes 1,800 grayscale images, six different types of typical surface defects each of which contains 300 samples. For defect detection tasks, the dataset provides annotations that indicate the category and location of the defect in each image. For each defect, the yellow box is the border indicating its location, and the green label is the category score.</p>

<div align=center><img src="https://user-images.githubusercontent.com/29084184/114502526-82306280-9c5e-11eb-9d60-011ee100e179.png"></div>


👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## Download
- Download ZIP, click [here](https://github.com/Charmve/Surface-Defect-Detection/archive/master.zip)
  <br>or run ```git clone https://github.com/Charmve/Surface-Defect-Detection.git``` in the terminal<br>
- Chinese Mainland - 百度网盘下载链接 https://pan.baidu.com/s/122WY8F5VKqm3qMirqebRQw ``提取码:i20n``

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## Notification

This work is originally contributed by lots of great man for their paper work or industry application. <strong>You can only use this dataset for research purpose.</strong>

If you have any questions or idea, please let me know :email: yidazhang1@gmail.com


## Citation
Use this bibtex to cite this repository:
```
@misc{Surface Defect Detection,
  title={Surface Defect Detection: Dataset and Papers},
  author={Charmve},
  year={2020.09},
  publisher={Github},
  journal={GitHub repository},
  howpublished={\url{https://github.com/Charmve/Surface-Defect-Detection}},
}
```
# Yolo-MSAPF
This project is the source and code for the paper titled “Yolo-MSAPF: Multi-Scale Alignment fusion with Parallel feature Filtering model for high accuracy weld defect detection”. We will upload the source and code after the paper is publicly published.

The first version of the dataset containing the original images appearing in the paper has been released.

### Table of Contents
![image](https://github.com/Luckycat518/Yolo-MSAPF/blob/main/Cover_image/Dataset-description.jpg)


The WSD-DET is collected from a commercial company. Therefore, this dataset is limited to academic use！！！Prohibited for any commercial use！！！

Before the entire dataset is fully released, if you need this dataset to do some research, please contact us. After review and permission by the commercial company, we will provide the dataset to you.


