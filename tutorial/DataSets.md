<!--
 * @Author: fanlong
 * @Date: 2022-09-29 10:06:53
 * @LastEditors: fanlong
 * @LastEditTime: 2023-03-27 13:29:51
 * @FilePath: \workspace_v10d:\01_paperNote-nju\DataSets.md
 * @Description: 
 * 
 * @github: https://github.com/fanl0228
 * @Email: fanl@smail.nju.edu.cn
 * Copyright (c) 2023 by fanlong/Nanjing University, All Rights Reserved. 
-->
# 数据集

---
# 毫米波雷达公开数据库

## [1.  NuScenes](https://www.nuscenes.org/nuscenes)


nuScenes数据集是一个具有3d对象标注的大规模自动驾驶数据集。包含了在波士顿和新加坡的1000个路况场景中采集的140万张图像（6个Camera），39万帧激光雷达数据（1个LiDAR），140万帧毫米波雷达数据（5个RADAR），以及在4万个关键帧中标注的140万个物体框。2020年7月还进一步发布了用于激光雷达语义分割的标注数据。它的特点:


- 全套传感器套件（1x LIDAR, 5x RADAR, 6x camera, IMU, GPS）
- 每20s有1000个场景
- Full sensor suite (1x LIDAR, 5x RADAR, 6x camera, IMU, GPS)
- 1000 scenes of 20s each
- 1,400,000 camera images
- 390,000 lidar sweeps
- Two diverse cities: Boston and Singapore
- Left versus right hand traffic
- Detailed map information
- 1.4M 3D bounding boxes manually annotated for 23 object classes
- Attributes such as visibility, activity and pose
- New: 1.1B lidar points manually annotated for 32 classes
- New: Explore nuScenes on SiaSearch
- Free to use for non-commercial use

<div style="text-align:center">
        <p align="center">
            <img src="imgs/DataSets/mmWare_Dataset_NuScenes.bmp", width="100%">
        </p>
    </div>

---
## [2.  CARRADA](ttps://github.com/valeoai/carrada_dataset)
这个数据库由法国的研究者于2020年首次发布，2021年又发布了新的版本。CARRADA包含了同步的图像和雷达数据，一共30个序列，12666帧（21.1分钟），其中7193帧包含标注的物体。标注的物体有三类，分别是行人，自行车和汽车。标注的格式有三种，分别是sparse point，bounding box和dense mask。CARRADA包含了底层的雷达数据，其格式为Range-Angle-Doppler Tensor。但是CARRADA的采集场景并不是真实的交通路况，因此其实用性会受到一定影响。

<div style="text-align:center">
        <p align="center">
            <img src="imgs/DataSets/mmWare_Dataset_CARRADA.png", width="100%">
        </p>
    </div>

---
## [3.  SCORP](https://sensorcortek.ai/paper-and-datasets/)
同样在2020年，加拿大，法国和德国的研究人员联合发布了SCORP数据库。这是第一个包含了ADC数据（经过数模转换后的I-Q samples）的公开数据库。ADC数据经过多次FFT处理后才得到RAD Tensor，因此SCORP的数据与CARRADA相比又更底层了一些。值得一提的是，这两个数据库的创建者中都包括了Valeo公司的研究人员。

SCORP数据库提供了三种数据表示，分别是Sample-Chirp-Angle (SCA) Tensor，Range-Azimuth-Doppler (RAD) Tensor以及Point Cloud。这三种数据来自雷达信号处理中的三个不同阶段。目前来说，机器学习算法常用的是Point Cloud，也有少量采用RAD Tensor的工作。这部分内容可以参考：[深度学习在毫米波雷达感知中的应用](https://zhuanlan.zhihu.com/p/362176955)

SCORP数据库包含了同步的图像数据，也用来辅助标注Free Space。针对这对三种不同的数据形式，作者测试了三种神经网络结构来试验Free Space Segmentation的效果。总的来说，SCORP是一个相对全面的数据库，但依然还存在三点不足：
- 1）数据量较少，只有来自11个序列的3913帧数据
- 2）没有BoundingBox标注，无法测试物体检测和跟踪算法
- 3）雷达和图像数据都来自于单个传感器，视场较窄，无法实现360度的感知


---
## [4. CRUW](https://www.cruwdataset.org/)
CRUW是一个用于自动驾驶汽车应用的公共相机-雷达数据集。这个数据库由华盛顿大学的研究者于2020年发布。这是一个相对大规模的数据库，包含了各种真实场景下（Parking lot，Campus road， City street， Highway）的40万帧图像和雷达数据。采集的传感器包括2个像机和2个雷达。CRUW提供了物体级别的标注，包括物体的位置，大小和类别，并且在图像数据上进一步提供了mask的信息。雷达数据的格式是Range-Azimuth Map。值得一提的是，作者基于此数据库发表了一个基准的多传感器融合物体检测算法，并且在2021年发布的基于此数据库的挑战比赛。</br></br>
**Rethinking of Radar’s Role: A Camera-Radar Dataset and
Systematic Annotator via Coordinate Alignment**

[paper](https://openaccess.thecvf.com/content/CVPR2021W/WAD/papers/Wang_Rethinking_of_Radars_Role_A_Camera-Radar_Dataset_and_Systematic_Annotator_CVPRW_2021_paper.pdf)</br>
[poster](http://yizhouwang.net/documents/wad_cvpr2021_poster.pdf)


---
## [5.  SeeingThroughFog](https://github.com/princeton-computational-imaging/SeeingThroughFog)
这个数据库包括了采用相机，毫米波雷达，激光雷达，热传感等多种传感器采集的超过10万个物体的数据。有意思的是，**这些数据是在极端的天气环境下采集**，包括雾天，雪天和雨天，来自于欧洲北部大约1万公里的行程。其目的是为了证明在极端天气环境下，多传感器的冗余性以及数据融合带来的性能提升。针对这一点，作者对比了很多方法，也提出了一种基于Entropy的融合算法</br>


[paper](https://arxiv.org/abs/1902.08913)



## 6. [毫米波汽车雷达原始ADC数据数据集（附MATLAB算法仿真）](https://github.com/Xiangyu-Gao/Raw_ADC_radar_dataset_for_automotive_object_detection)


---
# 唇读公开数据库

## [1. Lip Reading Datasets (Oxford)](http://www.robots.ox.ac.uk/~vgg/data/lip_reading/)
- LRW、LRS2和LRS3是在野生视频中采集的视听语音识别数据集。
- 6M+ word instances
- 800+ hours
- 5000+ identities







---
# 图像数据集
## [1. CIFAR](http://www.cs.toronto.edu/~kriz/cifar.html)


## [2. MNIST]()

## [3. ImageNet]()

## [4. COCO]()

