# Yolo-MSAPF<sup>📌</sup>
<a href="https://github.com/Luckycat518"><img src="https://img.shields.io/badge/GitHub-@Luckycat518-000000.svg?logo=GitHub" alt="GitHub" target="_blank"></a>
<a href="https://charmve.github.io/computer-vision-in-action/" target="_blank"><img src="https://img.shields.io/badge/Computer Vision-000000.svg?logo=GitBook" alt="Computer Vision in Action"></a>
[![License](https://img.shields.io/github/license/Charmve/Surface-Defect-Detection)](LICENSE)

# Table of Contents

- [Introduction](#introduction)
- [Key Problem in weld surface defect detection](#1-key-issues-in-weld-surface-defect-detection)
  - [External interference](#1external-impurity-interference)
  - [Adjacent interaction interference](#2adjacent-interaction-interference)
  - [Similarity interference](#3similarity-interference)
- [Our Dataset](#2-our-dataset-for-industrial-weld-surface-defect-detection)
  - [Weld Surface Defect: WSD-DET](#1weld-surface-defect-wsd-det)
- [Notification](#notification)
- [Citation](#citation)


## Introduction


<p>Up to now, many advanced deep-learning networks have been developed for the detection of weld surface defects. However, the detection speed and accuracy are still limited in the actual industrial environment because the weld surface defects are small and of many types. A great difficulty in location and classification will generate from these diverse small defects. In this work, to further promote the industrial application of the weld surface defect detection network, we aim to solve the industrial problems encountered in weld surface defect detection by providing specific improvement strategies. The fast-response Yolo-v5 model was selected as the baseline network to meet the real-time demand. Considering the existence of a huge amount of interference information on the weld surface, we designed a novel fusion strategy named multi-scale alignment fusion with parallel feature filtering (MSAPF) to integrate and filter multi-scale features. This strategy is implemented by multi-scale alignment fusion (MSAF) and parallel feature filtering (PFF) modules. The MSAF module aims to improve the problems of feature misalignment and spatial feature mismatch during multi-scale feature fusion by aligning features at one level to fuse all other scales. Thus, the sufficiency and accuracy of features are ensured. The subsequent PFF module simultaneously weights the channel and spatial features through the parallel dual-channel attention mechanism to efficiently screen the necessary features and filter out the interference features. Besides, other strategies are also applied to enhance the filtration performance and make lightweight of the whole model. Moreover, a dataset called <strong>WSD-DET</strong>, which covers the common defect categories occurring in the welding process, is built for weld surface defect detection. </p>



## 1. Key Issues in Weld Surface Defect Detection

### 1）External impurity interference

<p>Impurities such as welding slag on the surface of the weld will interfere with the judgment of the edge of the weld and the edge of the defect.</p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

### 2）Adjacent interaction interference

<p>It is highly possible to form a variety of defects with different scales on a weld, and these defects will overlap and interfere with each other when identifying their location and classification.</p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

### 3）Similarity interference
<p>The optical characteristics of some surface defects are similar. The types of these defects will be confused with each other when the contrast of optical features is not obvious.</p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## 2. Our dataset for Industrial Weld Surface Defect Detection

### 1）Weld Surface defect: WSD-DET

WSD-DET can be used for classification and positioning tasks.


<div align=center><img src="https://github.com/Luckycat518/Yolo-MSAPF/blob/main/Cover_image/Dataset-description.jpg"></div>

<p>The WSD-DET contains <b>7580</b> pictures with <b>8</b> types of defects were reserved. The defects for the original unpolished welds include weld_penetration, weld_beading,microporous, hole, incompletely_filled_groove, undercut, crazing and splash. The weld after grinding contains four kinds of defects: hole, undercut, crazing and weld_beading. </p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## Notification
<b>The first version of the dataset containing the original images appearing in the paper has been released.</b>
<p>The WSD-DET is collected from a commercial company. Therefore, this dataset is limited to academic use！！！Prohibited for any commercial use！！！
<strong>You can only use this dataset for research purpose.</strong>
Before the entire dataset is fully released, if you need this dataset to do some research, please contact us. After review and permission by the commercial company, we will provide the dataset to you.</p>


If you have any questions or idea, please let me know <p>(email: wgq001@csu.edu.cn)</p>

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)

## Citation
This paper is still under review......

👆 [<b>BACK to Table of Contents</b> -->](#table-of-contents)


<!-- LICENSE -->
## **License**

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

