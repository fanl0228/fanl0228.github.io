---
title: "2023-2024年浏览论文"
categories:
  - Markup
tags:
  - content
  - markup
toc: true
excerpt: 简要介绍浏览论文的摘要，核心思想，系统框架
---

## [Papaers path](https://box.nju.edu.cn/library/d0b874f1-ceda-4488-9318-7a487007e8a5/01_%E9%98%85%E8%AF%BB%E8%AE%BA%E6%96%87/2023_Extensive_Reading)




## 60.[mmWave-YOLO: A mmWave Imaging Radar-Based Real-Time Multiclass Object Recognition System for ADAS Applications](https://ieeexplore.ieee.org/document/9777730)
- **阅读时间：** 
- **Github**
- **出处：** IEEE Transactions on Instrumentation and Measurement 2022
- **关键词：** Advanced driver-assistance system (ADAS), imaging radar, millimeter wave (mmWave), neural networks, object recognition, sensor fusion
- **Abstract：** This article presents a millimeter wave (mmWave) imaging radar-based real-time multiclass object recognition system for advanced driver-assistance system (ADAS) applications related to construction machinery. While mmWave radar has the advantage of being able to detect signals even in the optically harsh, dark, and dusty environments in which construction machinery is often used, the radar has two orders of magnitude lower resolution than cameras. Since the distance from the radar increases, object features vary, resulting in making it difficult to classify and detect the location of multiple objects. To address this issue, an mmWave-you only look once (YOLO) architecture is proposed that enables highly accurate object classification and location recognition by applying different detectors to each distance data. To provide precise labels for the radar data semiautomatically, a camera-radar cooperative data annotator is also developed. Using the radar only, a real-time (46.6 ms) object classification and location detection of six class objects is achieved. The accuracy of our system is 84% [mean average precision (mAP)], which is slightly higher than that of the red, blue, green (RGB)-camera-based system (78%). In addition, since the radar can acquire similar data of target objects against any background, mmWave-YOLO can detect objects in a variety of scenes with only a small variation of the training dataset, resulting in a lower training cost. Experiments confirmed that it can detect objects in outdoor scenes even when it is trained only with indoor scene data.
- **摘要：**本文介绍了一种基于毫米波 (mmWave) 成像雷达的实时多类对象识别系统，适用于与工程机械相关的高级驾驶员辅助系统 (ADAS) 应用。 虽然毫米波雷达的优点是即使在工程机械经常使用的光学恶劣、黑暗和灰尘多的环境中也能检测到信号，但雷达的分辨率比摄像机低两个数量级。 由于与雷达的距离增加，物体特征发生变化，导致难以对多个物体进行分类和检测位置。 为了解决这个问题，提出了毫米波只看一次（YOLO）架构，该架构通过对每个距离数据应用不同的检测器来实现高精度的对象分类和位置识别。 为了半自动地为雷达数据提供精确的标签，还开发了摄像机-雷达协作数据注释器。 仅使用雷达，就实现了六类物体的实时（46.6 ms）物体分类和位置检测。 我们的系统的准确度为 84% [平均精度 (mAP)]，略高于基于红、蓝、绿 (RGB) 相机的系统 (78%)。 此外，由于雷达可以在任何背景下获取目标物体的相似数据，因此mmWave-YOLO可以在训练数据集变化很小的情况下检测各种场景中的物体，从而降低训练成本。 实验证实，即使仅使用室内场景数据进行训练，它也可以检测室外场景中的物体。
- **系统框架：** Camera and mmWave cooperative data annotation system.
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_60_fig1.png" alt="image" width ="100%">
    </div>


## 59.[mm-Wave Radar-Based Vital Signs Monitoring and Arrhythmia Detection Using Machine Learning](https://www.mdpi.com/1424-8220/22/9/3106)
- **阅读时间：** 
- **Github**
- **出处：** sensor article
- **关键词：**  mm-wave radar; artificial neural network; vital signs; machine learning
- **Abstract：** A non-contact, non-invasive monitoring system to measure and estimate the heart and breathing rate of humans using a frequency-modulated continuous wave (FMCW) mm-wave radar at 77 GHz is presented. A novel diagnostic system is proposed which extracts heartbeat phase signals from the FMCW radar (reconstructed using Fourier series analysis) to test a three-layer artificial neural network model to predict the presence of arrhythmia in individuals. The effect of person orientation, distance of measurement and movement was analyzed with respect to a reference device based on statistical measures that include number of outliers, mean, mean squared error (MSE), mean absolute error (MAE), median absolute error (medAE), skewness, standard deviation (SD) and R-squared values. The individual oriented in front of the radar outperformed almost all other orientations for most distances with an expected d = 90 cm and d = 120 cm. Furthermore, it was found that the heart rate that was measured while walking and the breathing rate which was measured for a motionless individual generated results with the lowest SD and MSE. An artificial neural network (ANN) was trained using the MIT-BIH database with a training accuracy of 93.9 % and an R2 value = 0.876. The diagnostic tool was tested on 15 subjects and achieved a mean test accuracy of 75%.
- **摘要：** 提出了一种非接触式、非侵入性监测系统，使用 77 GHz 的调频连续波 (FMCW) 毫米波雷达来测量和估计人类的心率和呼吸频率。 提出了一种新颖的诊断系统，该系统从 FMCW 雷达提取心跳相位信号（使用傅立叶级数分析重建）来测试三层人工神经网络模型，以预测个体是否存在心律失常。 基于统计测量，分析人的朝向、测量距离和移动相对于参考设备的影响，这些统计测量包括异常值数量、平均值、均方误差 (MSE)、平均绝对误差 (MAE)、中值绝对误差 (medAE)、偏度、标准差 (SD) 和 R 平方值。 在大多数距离（预期 d = 90 厘米和 d = 120 厘米）下，位于雷达前方的个体的表现优于几乎所有其他方向。 此外，还发现步行时测量的心率和静止个体测量的呼吸频率产生的 SD 和 MSE 最低。 使用 MIT-BIH 数据库训练人工神经网络 (ANN)，训练精度为 93.9%，R2 值 = 0.876。 该诊断工具在 15 名受试者身上进行了测试，平均测试准确率为 75%。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_59_fig1.png" alt="image" width ="100%">
    </div>



## 58.[MmWave Radar and Vision Fusion for Object Detection in Autonomous Driving: A Review](https://arxiv.org/abs/2108.03004)
- **阅读时间：** 
- **Github**
- **出处：**
- **关键词：** 
- **Abstract：** With autonomous driving developing in a booming stage, accurate object detection in complex scenarios attract wide attention to ensure the safety of autonomous driving. Millimeter wave (mmWave) radar and vision fusion is a mainstream solution for accurate obstacle detection. This article presents a detailed survey on mmWave radar and vision fusion based obstacle detection methods. First, we introduce the tasks, evaluation criteria, and datasets of object detection for autonomous driving. The process of mmWave radar and vision fusion is then divided into three parts: sensor deployment, sensor calibration, and sensor fusion, which are reviewed comprehensively. Specifically, we classify the fusion methods into data level, decision level, and feature level fusion methods. In addition, we introduce three-dimensional(3D) object detection, the fusion of lidar and vision in autonomous driving and multimodal information fusion, which are promising for the future. Finally, we summarize this article.
- **摘要：**随着自动驾驶的蓬勃发展，复杂场景下的精确目标检测受到广泛关注，以确保自动驾驶的安全。 毫米波（mmWave）雷达和视觉融合是精确障碍物检测的主流解决方案。 本文详细介绍了基于毫米波雷达和视觉融合的障碍物检测方法。 首先，我们介绍自动驾驶目标检测的任务、评估标准和数据集。 然后将毫米波雷达与视觉融合的过程分为传感器部署、传感器标定和传感器融合三个部分进行全面回顾。 具体来说，我们将融合方法分为数据级融合方法、决策级融合方法和特征级融合方法。 此外，我们还介绍了三维（3D）物体检测、自动驾驶中激光雷达和视觉的融合以及多模态信息融合，这些都是未来有前途的。 最后我们对这篇文章进行总结。
- **系统框架：**



## 57.[milliEgo: Single-chip mmWave Radar Aided Egomotion Estimation via Deep Sensor Fusion](https://arxiv.org/abs/2006.02266)
- **阅读时间：** 
- **Github**
- **出处：** Sensys2020
- **关键词：** 
- **Abstract：** Robust and accurate trajectory estimation of mobile agents such as people and robots is a key requirement for providing spatial awareness for emerging capabilities such as augmented reality or autonomous interaction. Although currently dominated by optical techniques e.g., visual-inertial odometry, these suffer from challenges with scene illumination or featureless surfaces. As an alternative, we propose milliEgo, a novel deep-learning approach to robust egomotion estimation which exploits the capabilities of low-cost mmWave radar. Although mmWave radar has a fundamental advantage over monocular cameras of being metric i.e., providing absolute scale or depth, current single chip solutions have limited and sparse imaging resolution, making existing point-cloud registration techniques brittle. We propose a new architecture that is optimized for solving this challenging pose transformation problem. Secondly, to robustly fuse mmWave pose estimates with additional sensors, e.g. inertial or visual sensors we introduce a mixed attention approach to deep fusion. Through extensive experiments, we demonstrate our proposed system is able to achieve 1.3% 3D error drift and generalizes well to unseen environments. We also show that the neural architecture can be made highly efficient and suitable for real-time embedded applications.
- **摘要：**人和机器人等移动代理的稳健而准确的轨迹估计是为增强现实或自主交互等新兴功能提供空间感知的关键要求。 尽管目前以视觉惯性里程计等光学技术为主，但这些技术面临场景照明或无特征表面的挑战。 作为替代方案，我们提出了 milliEgo，这是一种新颖的深度学习方法，可利用低成本毫米波雷达的功能进行稳健的自我运动估计。 尽管毫米波雷达比单目相机具有公制的基本优势，即提供绝对尺度或深度，但当前的单芯片解决方案的成像分辨率有限且稀疏，使得现有的点云配准技术变得脆弱。 我们提出了一种新的架构，该架构针对解决这一具有挑战性的姿势变换问题进行了优化。 其次，将毫米波姿态估计与附加传感器稳健地融合，例如 惯性或视觉传感器，我们引入了深度融合的混合注意力方法。 通过大量的实验，我们证明我们提出的系统能够实现 1.3% 的 3D 误差漂移，并能很好地推广到未见过的环境。 我们还表明，神经架构可以变得高效并且适合实时嵌入式应用。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_57_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. Our proposed milliEgo uses a low-cost COTS mmWave radar and IMU coupled with a deep neural network model to accurately and robustly estimate 6-DOF egomotion.We envision that milliEgo could be widely-integrated on mobile platforms to provide a high degree of spatial awareness to a wide range of applications.

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_57_fig2.png" alt="image" width ="100%">
    </div> 
    Fig.2. Overview of milliEgo, in which mmWave subnet and multi-modal fusion are two key submodules in its design. The default sensors of milliEgo is mmWave and IMU, it can also flexibly integrate the third sensor such as RGB or depth camera.

## 56.[Multi-Radar Inertial Odometry for 3D State Estimation using mmWave Imaging Radar](https://arxiv.org/abs/2311.08608)
- **阅读时间：** 
- **Github**
- **出处：** arXiv2023
- **关键词：** 毫米波成像雷达3D姿态估计
- **Abstract：** State estimation is a crucial component for the successful implementation of robotic systems, relying on sensors such as cameras, LiDAR, and IMUs. However, in real-world scenarios, the performance of these sensors is degraded by challenging environments, e.g. adverse weather conditions and low-light scenarios. The emerging 4D imaging radar technology is capable of providing robust perception in adverse conditions. Despite its potential, challenges remain for indoor settings where noisy radar data does not present clear geometric features. Moreover, disparities in radar data resolution and field of view (FOV) can lead to inaccurate measurements. While prior research has explored radar-inertial odometry based on Doppler velocity information, challenges remain for the estimation of 3D motion because of the discrepancy in the FOV and resolution of the radar sensor. In this paper, we address Doppler velocity measurement uncertainties. We present a method to optimize body frame velocity while managing Doppler velocity uncertainty. Based on our observations, we propose a dual imaging radar configuration to mitigate the challenge of discrepancy in radar data. To attain high-precision 3D state estimation, we introduce a strategy that seamlessly integrates radar data with a consumer-grade IMU sensor using fixed-lag smoothing optimization. Finally, we evaluate our approach using real-world 3D motion data.
- **摘要：**状态估计是成功实施机器人系统的关键组成部分，依赖于摄像头、激光雷达和 IMU 等传感器。 然而，在现实场景中，这些传感器的性能会因具有挑战性的环境而降低，例如， 恶劣的天气条件和弱光场景。 新兴的 4D 成像雷达技术能够在不利条件下提供强大的感知能力。 尽管具有潜力，但室内环境仍然面临挑战，因为嘈杂的雷达数据无法呈现清晰的几何特征。 此外，雷达数据分辨率和视场 (FOV) 的差异可能导致测量不准确。 虽然先前的研究已经探索了基于多普勒速度信息的雷达惯性里程计，但由于雷达传感器的视场和分辨率存在差异，3D 运动的估计仍然存在挑战。 在本文中，我们解决了多普勒速度测量的不确定性。 我们提出了一种优化身体框架速度同时管理多普勒速度不确定性的方法。 根据我们的观察，我们提出了一种双成像雷达配置，以减轻雷达数据差异的挑战。 为了实现高精度 3D 状态估计，我们引入了一种策略，使用固定滞后平滑优化将雷达数据与消费级 IMU 传感器无缝集成。 最后，我们使用真实世界的 3D 运动数据评估我们的方法。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_56_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. A demonstration of multi-radar inertial odometry (orange) walked through different levels of an atrium compared to visual-inertial odometry (green). The colors of the radar point cloud indicate Doppler velocity from high (red) to low (purple).


## 55.[Millimetro: mmWave retro-reflective tags for accurate, long range localization](https://dl.acm.org/doi/10.1145/3447993.3448627)
- **阅读时间：** 
- **Github**
- **出处：** MobiCom'21
- **关键词：** 
- **Abstract：** This paper presents Millimetro, an ultra-low-power tag that can be localized at high accuracy over extended distances. We develop Millimetro in the context of autonomous driving to efficiently localize roadside infrastructure such as lane markers and road signs, even if obscured from view, where visual sensing fails. While RF-based localization offers a natural solution, current ultra-low-power localization systems struggle to operate accurately at extended ranges under strict latency requirements. Millimetro addresses this challenge by re-using existing automotive radars that operate at mmWave frequency where plentiful bandwidth is available to ensure high accuracy and low latency. We address the crucial free space path loss problem experienced by signals from the tag at mmWave bands by building upon Van Atta Arrays that retro-reflect incident energy back towards the transmitting radar with minimal loss and low power consumption. Our experimental results indoors and outdoors demonstrate a scalable system that operates at a desirable range (over 100 m), accuracy (centimeter-level), and ultra-low-power (< 3 uW).
- **摘要：**本文介绍了 Millimetro，这是一种超低功耗标签，可以在长距离内进行高精度定位。 我们在自动驾驶的背景下开发 Millimetro，以有效地定位路边基础设施，例如车道标记和路标，即使在视觉传感失效的情况下，即使在视线模糊的情况下也是如此。 虽然基于射频的定位提供了一种自然的解决方案，但当前的超低功耗定位系统很难在严格的延迟要求下在扩展范围内准确运行。 Millitro 通过重复使用现有的汽车雷达来应对这一挑战，这些雷达以毫米波频率运行，有充足的带宽可确保高精度和低延迟。 我们通过构建 Van Atta 阵列来解决毫米波频段标签信号所遇到的关键自由空间路径损耗问题，该阵列以最小的损耗和低功耗将入射能量向后反射回发射雷达。 我们的室内和室外实验结果证明了一个可扩展的系统，可以在理想的范围（超过 100 m）、精度（厘米级）和超低功耗（< 3 uW）下运行。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_55_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. Millimetro is an ultra-low-power mmWave retroreflector that supports accurate localization at long-range. Millimetro gets its long-range from reflecting back incident waves directionally towards the reader, and accuracy from the large bandwidth available atmmWave.

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_55_fig2.png" alt="image" width ="100%">
    </div>
    Fig.2. System overview


## 54.[A Millimeter Wave Backscatter Network for Two-Way Communication and Localization](https://dl.acm.org/doi/10.1145/3603269.3604873)
- **阅读时间：** 
- **Github**
- **出处：** SigCom2023
- **关键词：** 
- **Abstract：** Millimeter wave (mmWave) technology enables wireless devices to communicate using very high-frequency signals. Operating at those frequencies provides larger bandwidth which can be used to enable high-data-rate links, and very accurate localization of devices. However, radios operating at high-frequencies consume significant amount of power, making them unsuitable for applications with limited energy sources. This paper presents MilBack, a backscatter network operating at mmWave bands. Backscattering is the most energy-efficient wireless communication technique, where nodes piggyback their data on an access point's signal instead of generating their own signals. Eliminating the need for signal generation significantly reduces the energy-consumption of the nodes. In contrast to past mmWave backscatter work which supports only uplink, MilBack is the first mmWave backscatter network which supports uplink, downlink, and accurate localization. MilBack addresses the key challenges that prevent existing backscatter networks to enable both uplink and downlink at mmWave bands. We implemented MilBack and evaluated its performance empirically. Our results show that MilBack is capable of achieving accurate localization, uplink, and downlink communication at up to 8 m while consuming only 32 mW and 18 mW, respectively.
- **摘要：** 毫米波 (mmWave) 技术使无线设备能够使用甚高频信号进行通信。 在这些频率下运行可提供更大的带宽，可用于实现高数据速率链路以及非常准确的设备定位。 然而，在高频下运行的无线电会消耗大量功率，因此不适合能源有限的应用。 本文介绍了 MilBack，一种在毫米波频段运行的反向散射网络。 反向散射是最节能的无线通信技术，其中节点将其数据搭载在接入点的信号上，而不是生成自己的信号。 消除信号生成的需要可以显着降低节点的能耗。 与过去仅支持上行链路的毫米波反向散射工作相比，MilBack是第一个支持上行链路、下行链路和精确定位的毫米波反向散射网络。 MilBack 解决了现有反向散射网络在毫米波频段上启用上行链路和下行链路的关键挑战。 我们实施了 MilBack 并根据经验评估了其性能。 我们的结果表明，MilBack 能够在长达 8 m 的距离内实现精确定位、上行链路和下行链路通信，而功耗分别仅为 32 mW 和 18 mW。
- **系统框架：**



## 53.[Contactless Blood Pressure Monitoring via Deep-Analyzed Hemodynamics](https)
- **阅读时间：** 
- **Github**
- **出处：**
- **关键词：** 毫米波雷达测血压，分析建模
- **Abstract：** Blood pressure (BP) measurement is significant to the assessment of many dangerous health conditions. Apart from invasively inserting catheters into arteries, non-invasive approaches typically rely on wearing devices on specific skin areas with consistent pressure. However, this can be uncomfortable and unsuitable for certain individuals, and the accuracy of these methods may significantly decrease due to improper device placements and wearing states. Recently, contactless methods leveraging RF technology have emerged as a potential alternative. However, these methods suffer from the drawback of overfitting deep learning (DL) models without a sound physiological basis, resulting in a lack of clear explanations for their outputs. Consequently, such limitations lead to skepticism and distrust among medical experts. In this paper, we propose hBP-Fi, a contactless BP measurement system driven by hemodynamics acquired via RF sensing. In addition to its contactless convenience, hBP-Fi is superior to other RF sensing approaches in i) grounding on hemodynamics as the key physical process of heart-pulse activities, ii) exploiting beam-steerable RF devices to achieve a super-resolution scan on the fine-grained pulse activities along arm arteries, and iii) ensuring the trustworthiness of system
outputs via an explainable (decision-understandable) DL model. Extensive experiments with 35 subjects demonstrate that hBP-Fi can achieve the error of -2.05±6.83mmHg and 1.99±6.30mmHg for monitoring systolic and diastolic blood pressures, respectively
- **摘要：** 血压 (BP) 测量对于评估许多危险的健康状况具有重要意义。 除了侵入性地将导管插入动脉外，非侵入性方法通常依赖于在特定皮肤区域以一致的压力佩戴设备。 然而，这对于某些人来说可能会感到不舒服和不适合，并且由于设备放置和佩戴状态不当，这些方法的准确性可能会显着降低。 最近，利用射频技术的非接触式方法已成为一种潜在的替代方案。 然而，这些方法存在过度拟合深度学习（DL）模型而没有健全的生理学基础的缺点，导致其输出缺乏清晰的解释。 因此，这种限制导致医学专家的怀疑和不信任。 在本文中，我们提出了 hBP-Fi，这是一种由射频传感获取的血流动力学驱动的非接触式血压测量系统。 除了非接触式便利性之外，hBP-Fi 还优于其他射频传感方法，i) 基于血流动力学作为心脏脉搏活动的关键物理过程，ii) 利用波束可控射频设备实现超分辨率扫描 沿手臂动脉的细粒度脉搏活动，以及 iii) 确保系统的可信度
通过可解释（决策可理解）的深度学习模型输出。 对35名受试者进行的大量实验表明，hBP-Fi在监测收缩压和舒张压方面的误差分别为-2.05±6.83mmHg和1.99±6.30mmHg
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_53_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. The concept of hBP-Fi: a path from hemodynamics understanding towards RF (micro-)motion sensing and explainable DL inference.

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_53_fig2.png" alt="image" width ="100%">
    </div>
    Fig.2. System overview



## 52.[mmTag: A MillimeterWave Backscatter Network](https://dl.acm.org/doi/10.1145/3452296.3472917)
- **阅读时间：** 
- **Github**
- **出处：** Sigcom'21
- **关键词：** 
- **Abstract：** Recent advances in IoT, machine learning and cloud computing have placed a huge strain on wireless networks. In particular, many emerging applications require streaming rich content (such as videos) in real time, while they are constrained by energy sources. A wireless network which supports high data-rate while consuming low-power would be very attractive for these applications. Unfortunately, existing wireless networks do not satisfy this requirement. For example, WiFi backscatter and Bluetooth networks have very low power consumption, but their data-rate is very limited (less than a Mbps). On the other hand, modern WiFi and mmWave networks support high throughput, but have a high power consumption (more than a watt). To address this problem, we present mmTag, a novel mmWave backscatter network which enables low-power high-throughput wireless links for emerging applications. mmTag is a backscatter system which operates in the mmWave frequency bands. mmTag addresses the key challenges that prevent existing backscatter networks from operating at mmWave bands. We implemented mmTag and evaluated its performance empirically. Our results show that mmTag is capable of achieving 1 Gbps and 100 Mbps at 4.6 m and 8 m, respectively, while consuming only 2.4 nJ/bit.
- **摘要：**物联网、机器学习和云计算的最新进展给无线网络带来了巨大的压力。 特别是，许多新兴应用程序需要实时传输丰富的内容（例如视频），但它们受到能源的限制。 支持高数据速率同时消耗低功耗的无线网络对于这些应用非常有吸引力。 不幸的是，现有的无线网络不能满足这个要求。 例如，WiFi 反向散射和蓝牙网络的功耗非常低，但它们的数据速率非常有限（小于 Mbps）。 另一方面，现代 WiFi 和毫米波网络支持高吞吐量，但功耗较高（超过一瓦）。为了解决这个问题，我们推出了 mmTag，这是一种新型毫米波反向散射网络，可为新兴应用提供低功耗高吞吐量无线链路。 mmTag 是一种在毫米波频段运行的反向散射系统。 mmTag 解决了阻止现有反向散射网络在毫米波频段运行的关键挑战。 我们实现了 mmTag 并根据经验评估了其性能。 我们的结果表明，mmTag 能够在 4.6 m 和 8 m 的距离上分别实现 1 Gbps 和 100 Mbps，而功耗仅为 2.4 nJ/bit。
- **系统框架：** 





## 51.[Rotation Speed Sensing with mmWave Radar]()
- **阅读时间：** 
- **Github:**
- **出处：** Infocom'2023
- **关键词：** 
- **Abstract：** Machines with rotary parts are prevalent in industrial systems and our daily lives. Rotation speed measurement is a crucial task for monitoring machinery health. Previous approaches for rotation speed sensing are constrained by limited operation distance, strict requirement for illumination, or strong dependency on the target object’s light reflectivity. In this work, we propose mRotate, a practical mmWave radar-based rotation speed sensing system liberated from all the above constraints. Specifically, mRotate separates the target signal reflected by the rotating object from the mixed reflection signals, extracts the high-quality rotation related features, and accurately obtains the rotation speed through the customized radar sensing mode and algorithm design. We implement mRotate on a commercial mmWave radar and extensively evaluate it in both lab environments and in a machining workshop for field tests. mRotate achieves an MAPE of 0.24% in accuracy test, which is 38% lower than that produced by the baseline device, a popular commercial laser tachometer. Besides, our experiments show that mRotate can measure a spindle whose diameter is only 5mm, maintain a high accuracy with a sensing distance as far as 2.5m, and simultaneously measure the rotation speeds of multiple objects.
- **摘要：** 带有旋转部件的机器在工业系统和我们的日常生活中普遍存在。 转速测量是监测机械健康状况的一项重要任务。 先前的转速感测方法受到操作距离有限、对照明的严格要求或对目标物体的光反射率的强烈依赖性的限制。 在这项工作中，我们提出了 mRotate，这是一种实用的基于毫米波雷达的旋转速度传感系统，摆脱了上述所有限制。 具体来说，mRotate从混合反射信号中分离出旋转物体反射的目标信号，提取高质量的旋转相关特征，并通过定制的雷达感知模式和算法设计，准确获取旋转速度。 我们在商用毫米波雷达上实施 mRotate，并在实验室环境和加工车间进行广泛评估以进行现场测试。 mRotate 在精度测试中实现了 0.24% 的 MAPE，比流行的商用激光转速计基准设备低 38%。 此外，我们的实验表明，mRotate可以测量直径仅为5mm的主轴，保持高精度，感应距离可达2.5m，同时测量多个物体的旋转速度。
- **系统框架：** 提出新的特征IFP(index of the first peak),建立雷达特征与旋转速度的关系。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_51_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. System overview.


## 50.[MetaWave: Attacking mmWave Sensing with Meta-material-enhanced Tags](https://www.ndss-symposium.org/ndss-paper/metawave-attacking-mmwave-sensing-with-meta-material-enhanced-tags/)
- **阅读时间：** 
- **Github**
- **出处：**
- **关键词：** 
- **Abstract：** Millimeter-wave (mmWave) sensing has been applied in many critical applications, serving millions of thousands of people around the world. However, it is vulnerable to attacks in the real world. These attacks are based on expensive and professional radio frequency (RF) modulator-based instruments and can be prevented by conventional practice (e.g., RF fingerprint). In this paper, we propose and design a novel passive mmWave attack, called MetaWave, with low-cost and easily obtainable meta-material tags for both vanish and ghost attack types. These meta-material tags are made of commercial off-the-shelf (COTS) materials with customized tag designs to attack various goals, which considerably low the attack bar on mmWave sensing. Specifically, we demonstrate that tags made of ordinal material (e.g., C-RAM LF) can be leveraged to precisely tamper the mmWave echo signal and spoof the range, angle, and speed sensing measurements. Besides, to optimize the attack, a general simulator-based MetaWave attack framework is proposed and designed to simulate the tag modulation effects on the mmWave signal with advanced tag and scene parameters. We evaluate, MetaWave, the meta-material tag attack in both simulation and real-world experiments (i.e., 20 different environments) with various attack settings. Experimental results demonstrate that MetaWave can achieve up to 97% Top-1 attack accuracy on range estimation, 96% on angle estimation, and 91% on speed estimation in actual practice, 10-100X cheaper than existing mmWave attack methods. We also evaluate the usability and robustness of MetaWave under different real-world scenarios. Moreover, we conduct in-depth analysis and discussion on countermeasures for MetaWave mmWave attacks to improve wireless sensing and cyber-infrastructure security.
- **摘要：**毫米波 (mmWave) 传感已应用于许多关键应用，为全球数以百万计的人们提供服务。 然而，它在现实世界中很容易受到攻击。 这些攻击基于昂贵且专业的基于射频 (RF) 调制器的仪器，并且可以通过传统做法（例如 RF 指纹）来预防。 在本文中，我们提出并设计了一种新型被动毫米波攻击，称为 MetaWave，具有低成本且易于获得的超材料标签，适用于消失和幽灵攻击类型。 这些超材料标签由商用现成 (COTS) 材料制成，具有定制的标签设计，可以攻击各种目标，从而大大降低了毫米波传感的攻击门槛。 具体来说，我们证明了由普通材料（例如 C-RAM LF）制成的标签可用于精确篡改毫米波回波信号并欺骗范围、角度和速度传感测量。 此外，为了优化攻击，提出并设计了一种基于通用模拟器的MetaWave攻击框架，以利用高级标签和场景参数来模拟毫米波信号上的标签调制效果。 我们在模拟和现实实验（即 20 个不同的环境）中使用各种攻击设置来评估 MetaWave 超材料标签攻击。 实验结果表明，MetaWave 在实际应用中可以实现高达 97% 的距离估计、96% 的角度估计和 91% 的速度估计的 Top-1 攻击精度，比现有毫米波攻击方法便宜 10-100 倍。 我们还评估了 MetaWave 在不同现实场景下的可用性和鲁棒性。 此外，我们还对MetaWave毫米波攻击的对策进行了深入的分析和讨论，以提高无线传感和网络基础设施的安全性。
- **系统框架：**




## 49.[milliEye: A Lightweight mmWave Radar and Camera Fusion System for Robust Object Detection](https://www.semanticscholar.org/paper/milliEye%3A-A-Lightweight-mmWave-Radar-and-Camera-for-Shuai-Shen/8868779625b1b88b5b077f31e69a74e76eb3d82e)
- **阅读时间：** 
- **Github** https://github.com/sxontheway/milliEye
- **出处：** IoTDI’21
- **关键词：** yolov3 + mmWave radar 融合实现目标检测；决策端融合（Figure 2 right）
- **Abstract：** A wide range of advanced deep learning algorithms have recently been proposed for image classification and object detection. However, the effectiveness of these methods can be significantly restricted in many real-world scenarios where the visibility or illumination is poor. Compared to RGB cameras, millimeter-wave (mmWave) radars are immune to the above environmental variability and can assist cameras under adverse conditions. To this end, we propose milliEye, a lightweight mmWave radar and camera fusion system for robust object detection on the edge platforms. milliEye has several key advantages over existing sensor fusion approaches. First, while milliEye fuses two sensing modalities in a learning-based fashion, it requires only a small amount of labeled image/radar data of a new scene as it can fully utilize large public image datasets for extensive training. This salient feature enables milliEye to adapt to highly complex real-world environments. Second, based on a novel architecture that decouples the image-based object detector from other modules, milliEye is compatible with different off-the-shelf image-based object detectors. As a result, it can take advantage of the rapid progress of object detection algorithms. Moreover, thanks to the highly compute-efficient fusion approach, milliEye is lightweight and thus suitable for edge-based real-time applications. To evaluate the performance of milliEye, we collect a new radar and camera fusion dataset for object detection, which contains both ordinary-light and low-light illumination conditions. The results show that milliEye can provide substantial performance boosts over state-of-the-art image-based object detectors, including Tiny YOLOv3 and SSD, especially in low-light scenes, while incurring low compute overhead on edge platforms.
- **摘要：** 最近提出了各种用于图像分类和对象检测的先进深度学习算法。 然而，在许多能见度或照明较差的现实场景中，这些方法的有效性可能会受到严重限制。 与 RGB 摄像头相比，毫米波 (mmWave) 雷达不受上述环境变化的影响，可以在不利条件下为摄像头提供帮助。 为此，我们提出了 milliEye，这是一种轻量级毫米波雷达和摄像头融合系统，用于在边缘平台上进行稳健的物体检测。 与现有传感器融合方法相比，milliEye 具有几个关键优势。 首先，虽然 milliEye 以基于学习的方式融合了两种传感模式，但它只需要新场景的少量标记图像/雷达数据，因为它可以充分利用大型公共图像数据集进行广泛的训练。 这一显着功能使 milliEye 能够适应高度复杂的现实环境。 其次，基于将基于图像的目标检测器与其他模块解耦的新颖架构，milliEye 与不同的现成基于图像的目标检测器兼容。 因此，它可以利用物体检测算法的快速进步。 此外，得益于计算效率高的融合方法，milliEye 重量轻，因此适合基于边缘的实时应用。 为了评估 milliEye 的性能，我们收集了用于目标检测的新雷达和相机融合数据集，其中包含普通光和低光照明条件。 结果表明，与最先进的基于图像的目标检测器（包括 Tiny YOLOv3 和 SSD）相比，milliEye 可以提供显着的性能提升，尤其是在低光场景中，同时在边缘平台上产生较低的计算开销。
- **系统框架：** 提出新的特征IFP(index of the first peak),建立雷达特征与旋转速度的关系。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_49_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. Left: conventional camera and radar fusion architecture that requires a large labeled image and radar dataset (> 10,000 frames) for training. Right: our proposed fusion architecture which enables separated weight training. Imagerelevant layers are trained on the large image dataset. Radarrelevant layers and scenario-agnostic result-level fusion layers are trained on the small customized multi-modality dataset (< 1,000 frames).



## 48. [Robust Hybrid Beamforming Design for Multi-RIS Assisted MIMO System With Imperfect CSI](https://ieeexplore.ieee.org/document/9957104)
- **阅读时间：** 
- **出处：** IEEE TRANSACTIONS ON WIRELESS COMMUNICATIONS (IEEE TWC) JCR Q1
- **关键词：** 
- **Abstract：** Reconfigurable intelligent surface (RIS) has been developed as a promising approach to enhance the performance of fifth-generation (5G) systems through intelligently reconfiguring the reflection elements. However, RIS-assisted beamforming design highly depends on the channel state information (CSI) and RIS’s location, which could have a significant impact on system performance. In this paper, the robust beamforming design is investigated for a RIS-assisted multiuser millimeter wave system with imperfect CSI, where the weighted sum-rate maximization problem (WSM) is formulated to jointly optimize transmit beamforming of the BS, RIS placement and reflect beamforming of the RIS. The considered WSM maximization problem includes CSI error, phase shifts matrices, transmit beamforming as well as RIS placement variables, which results in a complicated nonconvex problem. To handle this problem, the original problem is divided into a series of subproblems, where the location of RIS, transmit/reflect beamforming and CSI error are optimized iteratively. Then, a multiobjective evolutionary algorithm is introduced to gradient projection-based alternating optimization, which can alleviate the performance loss caused by the effect of imperfect CSI. Simulation results reveal that the proposed scheme can potentially enhance the performance of existing wireless communication, especially considering a desirable trade-off among beamforming gain, user priority and error factor.
- **摘要：** 可重构智能表面 (RIS) 已被开发为一种很有前途的方法，可通过智能地重新配置反射元件来增强第五代 (5G) 系统的性能。 然而，RIS 辅助波束成形设计高度依赖于信道状态信息 (CSI) 和 RIS 的位置，这可能对系统性能产生重大影响。 本文研究了具有不完善 CSI 的 RIS 辅助多用户毫米波系统的鲁棒波束成形设计，其中制定了加权和速率最大化问题（WSM）来联合优化 BS 的发射波束成形、RIS 放置和反射波束成形 RIS 的。 考虑的WSM最大化问题包括CSI误差、相移矩阵、发射波束成形以及RIS放置变量，这导致复杂的非凸问题。 为了处理这个问题，原始问题被分为一系列子问题，其中RIS的位置、发射/反射波束成形和CSI误差被迭代优化。 然后，将多目标进化算法引入基于梯度投影的交替优化，可以减轻由于CSI不完善的影响而造成的性能损失。 仿真结果表明，所提出的方案可以潜在地增强现有无线通信的性能，特别是考虑到波束成形增益、用户优先级和误差因子之间的理想权衡。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_48_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. Illustration of the considered multi-RIS-assisted MIMO communication system.


## 47. [Towards Position-Independent Sensing for Gesture Recognition with Wi-Fi](https://dl.acm.org/doi/10.1145/3463504)
- **阅读时间：** 2023-09-19
- **出处：** UbiComp'21
- **关键词：** wifi，手势识别
- **摘要：** Past decades have witnessed the extension of the Wi-Fi signals as a useful tool sensing human activities. One common assumption behind it is that there is a one-to-one mapping between human activities and Wi-Fi received signal patterns. However, this assumption does not hold when the user conducts activities in different locations and orientations. Actually, the received signal patterns of the same activity would become inconsistent when the relative location and orientation of the user with respect to transceivers change, leading to unstable sensing performance. This problem is known as the position-dependent problem, hindering the actual deployment of Wi-Fi-based sensing applications. In this paper, to tackle this fundamental problem, we develop a new position-independent sensing strategy and use gesture recognition as an application example to demonstrate its effectiveness. The key idea is to shift our observation from the traditional transceiver view to the hand-oriented view, and extract features that are irrespective of position-specific factors. Following the strategy, we design a position-independent feature, denoted as Motion Navigation Primitive(MNP). MNP captures the pattern of moving direction changes of the hand, which shares consistent patterns when the user performs the same gesture with different position-specific factors. By analyzing the pattern of MNP, we convert gestures into sequences of strokes (e.g, line, arc and corner) which makes them easy to be recognized. We build a prototype WiFi gesture recognition system, i.e., WiGesture to validate the effectiveness of the proposed strategy. Experiments show that our system can outperform the start-of-arts significantly in different settings. Given its novelty and superiority, we believe the proposed method symbolizes a major step towards gesture recognition and would inspire other solutions to position-independent activity recognition in the future.

- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_47_fig1.png" alt="image" width ="100%">
    </div>
    Fig.1. Illustrations of Drawing ’2’ with Different Position-specific Factors



- **学习的点：**
    1. 利用不同天线信号比值提取动态相位，Extract the Dynamic Phase Changes from the CSI, 如公式(8).
    2. 


## 46. [Towards Robust Gesture Recognition by Characterizing the Sensing Quality of WiFi Signals](https://www.researchgate.net/publication/359586964_Towards_Robust_Gesture_Recognition_by_Characterizing_the_Sensing_Quality_of_WiFi_Signals)
- **阅读时间：** 
- **出处：** Ubicomp‘22
- **关键词：** gesture recognition; wifi
- **摘要：** WiFi-based gesture recognition emerges in recent years and attracts extensive attention from researchers. Recognizing gestures via WiFi signal is feasible because a human gesture introduces a time series of variations to the received raw signal. The major challenge for building a ubiquitous gesture recognition system is that the mapping between each gesture and the series of signal variations is not unique, exact the same gesture but performed at different locations or with different orientations towards the transceivers generates entirely different gesture signals (variations). To remove the location dependency, prior
work proposes to use gesture-level location-independent features to characterize the gesture instead of directly matching the
signal variation pattern. We observe that gesture-level features cannot fully remove the location dependency since the signal
qualities inside each gesture are different and also depends on the location. Therefore, we divide the signal time series of
each gesture into segments according to their qualities and propose customized signal processing techniques to handle them
separately. To realize this goal, we characterize signal’s sensing quality by building a mathematical model that links the gesture
signal with the ambient noise, from which we further derive a unique metric i.e., error of dynamic phase index (EDP-index) to
quantitatively describe the sensing quality of signal segments of each gesture. We then propose a quality-oriented signal
processing framework that maximizes the contribution of the high-quality signal segments and minimizes the impact of
low-quality signal segments to improve the performance of gesture recognition applications. We develop a prototype on
COTS WiFi devices. The extensive experimental results demonstrate that our system can recognize gestures with an accuracy
of more than 94% on average, and significant improvements compared with state-of-arts.

- **引用** </br> 
  
    ```
    @article{10.1145/3517241,
    author = {Gao, Ruiyang and Li, Wenwei and Xie, Yaxiong and Yi, Enze and Wang, Leye and Wu, Dan and Zhang, Daqing},
    title = {Towards Robust Gesture Recognition by Characterizing the Sensing Quality of WiFi Signals},
    year = {2022},
    issue_date = {March 2022},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    volume = {6},
    number = {1},
    url = {https://doi.org/10.1145/3517241},
    doi = {10.1145/3517241},
    abstract = {WiFi-based gesture recognition emerges in recent years and attracts extensive attention from researchers. Recognizing gestures via WiFi signal is feasible because a human gesture introduces a time series of variations to the received raw signal. The major challenge for building a ubiquitous gesture recognition system is that the mapping between each gesture and the series of signal variations is not unique, exact the same gesture but performed at different locations or with different orientations towards the transceivers generates entirely different gesture signals (variations). To remove the location dependency, prior work proposes to use gesture-level location-independent features to characterize the gesture instead of directly matching the signal variation pattern. We observe that gesture-level features cannot fully remove the location dependency since the signal qualities inside each gesture are different and also depends on the location. Therefore, we divide the signal time series of each gesture into segments according to their qualities and propose customized signal processing techniques to handle them separately. To realize this goal, we characterize signal's sensing quality by building a mathematical model that links the gesture signal with the ambient noise, from which we further derive a unique metric i.e., error of dynamic phase index (EDP-index) to quantitatively describe the sensing quality of signal segments of each gesture. We then propose a quality-oriented signal processing framework that maximizes the contribution of the high-quality signal segments and minimizes the impact of low-quality signal segments to improve the performance of gesture recognition applications. We develop a prototype on COTS WiFi devices. The extensive experimental results demonstrate that our system can recognize gestures with an accuracy of more than 94\% on average, and significant improvements compared with state-of-arts.},
    journal = {Proc. ACM Interact. Mob. Wearable Ubiquitous Technol.},
    month = {mar},
    articleno = {11},
    numpages = {26},
    keywords = {Human-Computer Interaction (HCI), Gesture Recognition, Wireless Sensing}
    }
    ```
    
- **单词、句子：** </br> 
  
    - In this section, we investigate the phenomenon of different sensing quality which influences the robustness of gesture recognition.


- **系统框架：** Flowchart of our proposed framework of SSL gesture recognition system.
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_46_fig1.png" alt="image" width ="100%">
    </div> 

- **关注点：**
    1. 手势信号质量评估标准的 的理解
    2. DPSense - EDP-index信号质量评价指标，用于评估手势什么情况下信号质量最强，如论文中的Fig.8
    3. 
    


## 45. [Chapter 11- WiFi CSI-based vital signs monitoring](https://www.sciencedirect.com/science/article/pii/B9780128222812000202)
- **整理时间：** 2023-3-25
- **出处：** Contactless Vital Signs Monitoring, 2022, Pages 231-255
- **关键词：** 
- **摘要：** 人体呼吸监测在医疗保健应用中发挥着重要作用，例如睡眠呼吸暂停检测和睡眠阶段识别。 我们见证了为呼吸监测开发的多种方法，从接触式脉搏血氧仪到非接触式摄像头和 CW（连续波）雷达解决方案。 最近，由于 WiFi 基础设施的普遍部署，基于 WiFi CSI 的非接触式传感解决方案吸引了大量研究关注。 在本章中，我们首先概述基于 WiFi 的人体呼吸监测技术，涵盖基于模式和基于模型的方法。 通过引入菲涅尔反射和衍射模型，我们随后展示了如何使用 WiFi 信号实现人体呼吸感应，以及为什么有时会出现使用 WiFi CSI 振幅的“盲点”。 针对单人呼吸监测的“盲点”和感应距离短的问题，我们进一步开发了一系列解决方案。 最后，我们还为多人呼吸感应提出了最先进的解决方案。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_45_fig1.png" alt="image" width ="80%">
    </div>


## 44. [The Role of Millimeter-Wave Technologies in 5G/6G Wireless Communications](https)
- **整理时间：** 2023-3-25
- **出处：** IEEE Journal of Microwaves ( Volume: 1, Issue: 1, January 2021)
- **关键词：** 
- **摘要：** 自从部署第一代移动通信以来，无线通信技术在过去四十年中以惊人的速度发展。 即将到来的第五代 (5G) 通过在移动通信基础设施中首次利用毫米波频谱，有望提供超快的数据速率、极低的延迟和显着提高的频谱效率。 在 2030 年以后的几年里，新出现的数据密集型应用和大幅扩展的无线网络将呼唤第六代 (6G) 通信，这是对 5G 网络的重大升级——几乎覆盖整个地球表面和近邻 外太空。 无论是在 5G 还是未来的 6G 网络中，毫米波技术都将在完成设想的网络性能和通信任务方面发挥重要作用。 本文综述了相关的毫米波使能技术：包括有源波束形成阵列、波束形成集成电路、基站和用户终端天线、系统测量和校准以及信道表征等系统架构的最新进展。 还简要讨论了各部分对未来6G通信的要求。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_44_fig1.png" alt="image" width ="80%">
    </div>
    

## 43. [The Visual Accelerometer: A High-fidelity Optic-to-Inertial Transformation Framework for Wearable Health Computing](https://ieeexplore.ieee.org/document/9874659)
- **整理时间：** 2023-3-25
- **出处：** 2022 IEEE 10th International Conference on Healthcare Informatics (ICHI)
- **关键词：** 
- **摘要：** 人类日常生活活动 (ADL) 监测已应用于生命关键应用，例如职业安全和中风康复跟踪。 然而，可穿戴计算作为ADL监测的主要技术范式，需要付出巨大的努力才能获得令人满意的带有标签的惯性数据用于训练。 在本文中，我们开发了 VisuaIAcc，这是一种用于可穿戴计算的人体运动的高保真光学惯性框架，它利用从公共视频中收集的光强度数据来重建真实的可穿戴运动数据。 具体来说，首先设计了一个两步光学运动估计器，以从时变光强度推断出高质量的光学运动场（OMF）。 然后，将获得的 OMF 馈送到光惯性转换器，该转换器利用光线投影中的人体运动学约束在基于卷积的过程中恢复时序惯性数据。 实验结果表明，通过 VisualAcc 重建的数据与来自真实的现成 MEMS 传感器的真实数据之间的皮尔逊相关系数超过 0.86。 此外，我们对 IMU 逆人体动力学分析进行了案例研究，以展示 VisualAcc 在增强和转变细粒度可穿戴计算方面的潜力。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_43_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_43_fig2.png" alt="image" width ="80%">
    </div> 



## 42. [Synthesized Millimeter-Waves for Human Motion Sensing](https://www.semanticscholar.org/paper/Synthesized-Millimeter-Waves-for-Human-Motion-Zhang-Li/3a0b4ad5db3b144ef8603963ab8b8157c9a53748)
- **整理时间：** 2023-3-25
- **出处：** SenSys ’22
- **关键词：** 
- **摘要：** 在这个项目中，我们展示了 SynMotion，这是一种新的基于毫米波的人体运动传感系统。 其新颖之处在于获取可用的基于视觉的人体运动数据集，了解不同运动下身体骨骼点的坐标，合成从人体反射回来的毫米波传感信号，使合成信号可以继承标签（骨骼坐标和 每个动作的名称）直接来自基于视觉的数据集。 SynMotion 展示了生成此类高质量标记合成数据的能力，以解决训练数据稀缺问题，并支持两种可与商用雷达配合使用的传感服务，包括 1) 零射击活动识别，其中分类器读取真实毫米波进行识别 ，但它只接受合成数据的训练； 2) 在真实毫米波上使用少量/零样本学习进行身体骨骼跟踪。 为了设计 SynMotion，我们解决了毫米波合成固有的复杂性以及与真实毫米波相比的微观差异的挑战。 大量实验表明，SynMotion 优于最新的基于零镜头毫米波的活动识别方法。 对于骨骼跟踪，SynMotion 实现了与在标记的毫米波上训练的最先进的基于毫米波的方法相当的性能，并且 SynMotion 可以在看不见的用户方面进一步超越它。

- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_42_fig1.png" alt="image" width ="80%">
    </div> 


## 41. [RoS: Passive Smart Surface for Roadside-to-Vehicle Communication](https://conferences.sigcomm.org/sigcomm/2021/files/papers/3452296.3472896.pdf)
- **整理时间：** 2023-3-25
- **出处：** SigComm'21
- **关键词：** 
- **摘要：** 现代自动驾驶汽车通常配备雷达以实现全天候感知。 然而，雷达的功能仅限于识别反射器在环境中的位置。 在本文中，我们研究了智能化交通基础设施的可行性，以便向汽车雷达传输更丰富的信息。 我们提出了 RoS，一种无源 PCB 制造的表面，可以通过机械方式重新配置以嵌入数字位，并像视觉路标对相机所做的那样通知雷达。 我们将 RoS 标牌设计为后向反射器，可以从宽视角将信号反射回雷达。 我们进一步介绍了一种空间编码方案，它根据回射元件的几何布局在反射模拟信号中搭载信息。 我们的原型制造和实验验证了 RoS 作为射频“条形码”的有效性，在实际运输环境中雷达可读取该条形码。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_41_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_41_fig2.png" alt="image" width ="80%">
    </div> 


## 40. [MoVi-Fi: Motion-robust Vital SignsWaveform Recovery via Deep Interpreted RF Sensing](https://dl.acm.org/doi/abs/10.1145/3447993.3483251)
- **整理时间：** 2023-3-25
- **出处：** Mobicom'21
- **关键词：** 
- **摘要：** 生命体征是人类健康的重要指标，研究人员正在研究现有可穿戴生命体征传感器的非接触式替代品。 不幸的是，这些设计中的大多数都要求主体人体相对静止，这使得它们在身体运动频繁发生的实践中采用起来非常不便。 特别是，基于射频 (RF) 的非接触式传感可能会受到压倒生命体征的身体运动的严重影响。 为此，我们引入了 MoVi-Fi 作为运动稳健的生命体征监测系统，能够以非接触方式恢复细粒度的生命体征波形。 作为一个纯软件系统，MoVi-Fi 几乎可以构建在任何商业级雷达之上。 激发我们设计灵感的是，由生命体征引起的射频反射虽然微弱，但并没有完全消失，而是与其他运动引起的反射以非线性方式合成。 由于非线性盲源分离本身就很困难，MoVi-Fi 创新地采用深度对比学习来解决这个问题； 这种自我监督的方法在训练中不需要基本事实，它利用对比信号特征来区分生命体征和身体运动。 我们对 12 名受试者和 80 小时数据进行的实验表明，MoVi-Fi 可以准确地恢复剧烈身体运动下的生命体征波形。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_40_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_40_fig2.png" alt="image" width ="80%">
    </div> 




## 39. [Mosaic: Leveraging Diverse Reflector Geometries for Omnidirectional Around-Corner Automotive Radar](https://dl.acm.org/doi/10.1145/3498361.3538944)
- **整理时间：** 2023-3-25 
- **出处：** MobiSys'22
- **关键词：** 

- **Abstract:** A large number of traffic collisions occur as a result of obstructed sight lines, such that even an advanced driver assistance system would be unable to prevent the crash. Recent work has proposed the use of around-the-corner radar systems to detect vehicles, pedestrians, and other road users in these occluded regions. Through comprehensive measurement, we show that these existing techniques cannot sense occluded moving objects in many important real-world scenarios. To solve this problem of limited coverage, we leverage multiple, curved reflectors to provide comprehensive coverage over the most important locations near an intersection. In scenarios where curved reflectors are insufficient, we evaluate the relative benefits of using additional flat planar surfaces. Using these techniques, we more than double the probability of detecting a vehicle near the intersection in three real urban locations, and enable NLoS radar sensing using an entirely new class of reflectors.

- **摘要：** 大量的交通事故都是由于视线受阻而发生的，即使是先进的驾驶辅助系统也无法避免碰撞。 最近的工作提出使用环角雷达系统来检测这些封闭区域中的车辆、行人和其他道路使用者。 通过综合测量，我们表明这些现有技术无法在许多重要的现实场景中感知被遮挡的移动物体。 为解决覆盖范围有限的问题，我们利用多个曲面反射器对交叉路口附近最重要的位置进行全面覆盖。 在曲面反射器不足的情况下，我们评估了使用额外平坦表面的相对优势。 使用这些技术，我们将在三个真实城市位置的十字路口附近检测到车辆的概率提高了一倍以上，并使用全新类别的反射器实现 NLoS 雷达感应。


- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_39_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_39_fig2.png" alt="image" width ="80%">
    </div> 



## 38. [MiShape: Accurate Human Silhouettes and Body Joints from Commodity Millimeter-Wave Devices](https://cse.sc.edu/~hregmi/pubs/journals/Aakriti_IMWUT22_MiShape.pdf)
- **整理时间：** 2023-3-25 
- **出处：** Upicomp'22
- **关键词：** 
- **摘要：** 我们提出了 MiShape，这是一种基于毫米波 (mmWave) 无线信号的成像系统，可生成高分辨率人体轮廓并预测身体关节的 3D 位置。 该系统可以在低光照和低能见度条件下实时捕捉人体动作。 与现有的基于视觉的运动捕捉系统不同，MiShape 是一种非侵入式隐私系统，可以推广到各种家庭运动跟踪应用。 为了克服商用现成 (COTS) 毫米波系统图像中的低分辨率、镜面反射和混叠等挑战，MiShape 设计了基于条件生成对抗网络的深度学习模型，并结合了人类生物力学规则。 我们为步态监测定制了 MiShape，但该模型可以很好地适应任何微调样本有限的跟踪应用。 我们使用从 COTS 毫米波系统收集的真实数据对 MiShape 进行实验性评估，这些数据来自 10 名年龄、性别、身高和体型各不相同、姿势各异的志愿者。 我们的实验结果表明，MiShape 可提供与现有基于视觉的系统相当的高分辨率轮廓和准确的身体姿势，并释放毫米波系统（例如 5G 家庭无线路由器）在隐私非侵入性医疗保健应用中的潜力。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_38_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_38_fig2.png" alt="image" width ="80%">
    </div> 


## 37. [Through](https)
- **整理时间：** 2023-3-25
- **出处：** 
- **关键词：** 
- **摘要：** 

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/png" alt="image" width ="80%">
    </div> 




## 36. [Millimetro:mmWave Retro-Reflective Tags for Accurate, Long Range Localization](https)
- **整理时间：** 2023-3-25
- **出处：** MobiCom'21
- **关键词：** 
- **摘要：** 本文介绍了 Millimetro，这是一种超低功耗标签，可以在远距离上以高精度定位。 我们在自动驾驶的背景下开发 Millimetro，以有效地定位路边基础设施，例如车道标记和道路标志，即使在视觉感应失败的地方被遮挡。 虽然基于 RF 的定位提供了一种自然的解决方案，但当前的超低功耗定位系统难以在严格的延迟要求下在扩展范围内准确运行。 Millimetro 通过重新使用以毫米波频率运行的现有汽车雷达来应对这一挑战，其中有足够的带宽可确保高精度和低延迟。 我们通过构建 Van Atta 阵列来解决毫米波频段标签信号遇到的关键自由空间路径损耗问题，该阵列将入射能量反向反射回发射雷达，损耗最小且功耗低。 我们在室内和室外的实验结果展示了一个可扩展的系统，该系统在理想的范围（超过 100 米）、精度（厘米级）和超低功耗（< 3 uW）下运行。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_36_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_36_fig2.png" alt="image" width ="80%">
    </div> 




## 35. [Millimeter Wave Wireless Communications: New Results for Rural Connectivity](https://arxiv.org/pdf/1608.05384v2.pdf)
- **整理时间：** 2023-3-25
- **出处：** ATC'16
- **关键词：** 
- **摘要：** 本文展示了使用毫米波通信可以实现的显着距离，并基于弗吉尼亚农村地区 73 GHz 的测量结果，提出了一种新的毫米波频率农村宏蜂窝 (RMa) 路径损耗模型。 需要路径损耗模型来估计无线网络设计的信号覆盖范围和干扰，但人们对毫米波的农村传播知之甚少。 这项工作确定了第三代合作伙伴计划 (3GPP) TR 38.900 第 14 版使用的 RMa 模型的问题，并提供了一个近距离 (CI) 参考距离模型，与 现有的 3GPP RMa 路径损耗模型。 此处介绍的测量和模型是第一个验证农村毫米波路径损耗模型的方法。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_35_fig1.png" alt="image" width ="80%">
    </div>


## 34. [M5: Facilitating Multi-user Volumetric Content Delivery with Multi-lobe Multicast over mmWave](https://dl.acm.org/doi/pdf/10.1145/3560905.3568540)
- **整理时间：** 2023-3-25
- **出处：** SenSys ’22
- **关键词：** 
- **摘要：** 多用户体积内容交付可以实现许多有吸引力的应用程序，例如在线教育、远程医疗、多用户 AR/VR 培训、沉浸式协作分析等。但是，体积视频流的带宽密集型特性使得现有系统只能提供单用户体验 难以扩展到多用户场景。 为了解决这个关键问题，在本文中，我们首先在提供所需的多 Gbps 吞吐量的毫米波网络上进行扩展实验，并确定向多个用户流式传输高质量体积视频的两个关键挑战：毫米波链路的频繁阻塞和高 用户之间的传输冗余。 为了解决这些问题，我们提出了一个同类首创的敏捷跨层系统，称为 M5，用于提高多用户体积视频流的性能和体验质量。 M5 利用用户的 6DoF 运动预测来主动调整毫米波波束和预取帧以减轻阻塞影响。 此外，它利用多播传输的优势，在用户的视口内传送重叠的公共内容，以减少带宽需求。 我们在真实测试台和跟踪驱动模拟器上进行的大量实验表明，与最先进的系统相比，M5 可以有效地将帧速率提高 44.1%，将体积视频质量提高 62.3%。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_34_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_34_fig2.png" alt="image" width ="80%">
    </div> 




## 33. [M4esh: mmWave-based 3D Human Mesh Construction for Multiple Subjects](https://www.semanticscholar.org/paper/M4esh%3A-mmWave-Based-3D-Human-Mesh-Construction-for-Xue-Cao/b16485978054b3dc18fb8bcca406d81768623864)
- **整理时间：** 2023-3-25
- **出处：** SenSys ’22,
- **关键词：** 毫米波实现3D人体网格建模
- **摘要：** 最近各种无线传感系统和应用的激增证明了射频 (RF) 信号优于传统的基于摄像头的解决方案，后者面临着各种挑战，例如遮挡和光线条件不佳。 为实现使用射频信号对人体成像的最终目标，研究人员一直在探索构建人体网格的可能性，人体网格是一种从射频信号中捕捉人体姿势和形状的结构。 在本文中，我们介绍了 M4esh，这是一种利用商用毫米波 (mmWave) 雷达进行多主体 3D 人体网格构建的新型系统。 我们的 M4esh 系统可以通过预测地图上的主体边界框来检测和跟踪 2D 能量图上的主体，并通过利用先前帧中主体边界框的位置、速度和大小信息来解决主体的相互遮挡 作为估计当前帧中边界框的线索。 通过在真实世界的 COTS 毫米波测试台上进行大量实验，我们表明我们提出的 M4esh 系统可以准确定位对象并生成他们的人体网格，这证明了所提出的 M4esh 系统的卓越有效性。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_33_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_33_fig2.png" alt="image" width ="80%">
    </div> 

- **Mesh Estimation Model:**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_33_fig3.png" alt="image" width ="80%">
    </div> 


## 32. [IndexPen: Two-Finger Text Input with Millimeter-Wave Radar](https://www.researchgate.net/publication/361826003_IndexPen_Two-Finger_Text_Input_with_Millimeter-Wave_Radar)
- **整理时间：** 2023-3-25
- **出处：** UbiComp'22
- **关键词：** 毫米波FMCW雷达； 微手势感应； 空中手势； 深度学习； 文字输入； 光标交互
- **摘要：** 在本文中，我们介绍了 IndexPen，这是一种通过双指空中微手势进行文本输入的新颖交互技术，可实现免触摸、轻松、基于跟踪的交互，旨在反映真实世界的书写。 我们的系统基于毫米波雷达传感，不需要用户使用仪器。 IndexPen 可以成功识别 30 种不同的手势，代表字母 A-Z，以及 Space、Backspace、Enter 和一种特殊的 Activation 手势，以防止无意输入。 此外，我们还包括一个噪声类来区分手势和非手势噪声。 我们展示了我们的系统设计，包括射频 (RF) 处理管道、分类模型和实时检测算法。 我们进一步展示了我们的概念验证系统，其中收集了十天的数据，五名参与者在 31 个类别（包括噪音）上产生了 95.89% 的交叉验证准确率。 此外，我们与 16 名首次使用 IndexPen 的参与者一起探索了我们的系统对真实世界文本输入的可学习性和适应性，共计 5 次。 每次会议结束后，之前的五用户研究中的预训练模型都会根据迄今为止通过迁移学习为新用户收集的数据进行校准。 F-1 分数显示每次校准后会话平均增加 9.14%，在最后一次会话中 16 个用户平均达到 88.3%。 同时，我们表明用户可以使用 IndexPen 以 86.2% 的准确率键入句子，这是通过字符串相似性来衡量的。 这项工作为未来的交互界面奠定了基础和愿景，可以通过这种范式实现。

- **应用场景：** </br> IndexPen 可在物理尺寸有限且无需佩戴仪器的设备上实现空中双指文本输入。 例如，它可以在 ATM 等公共设备上提供非接触式打字界面，以改善卫生状况。 它提供了在小屏幕上打字的替代方案，在小屏幕上打字很困难，语音输入不合适或不可行。 IndexPen 识别类似于手写的手势，包括 30 个类别。 该系统处理微型雷达设备生成的速度和角度轮廓，并使用神经网络检测手势。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_32_fig1.png" alt="image" width ="80%">
    </div>
    
- **实验系统：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_32_fig2.png" alt="image" width ="80%">
    </div> 

## 31. [High-Dimensional MVDR Beamforming: Optimized Solutions Based on Spiked Random Matrix Models](https)
- **整理时间：** 2023-3-25
- **出处：** IEEE Transactions on Signal Processing ( Volume: 66, Issue: 7, 01 April 2018)
- **关键词：** 
- **摘要：** 最小方差无失真响应 (MVDR) 波束成形（或 Capon 波束成形）是最流行的自适应阵列处理策略之一，因为它能够在消除干扰的同时提供抗噪能力。 这种波束形成器的一个实际挑战是它涉及接收信号的逆协方差矩阵，必须根据数据进行估计。 在现代高维应用中，众所周知，经典估计器会受到采样噪声的严重影响，从而影响波束形成器的性能。 在这里，我们提出了一种适用于高维设置的 MVDR 波束形成新方法。 特别是，通过与 MVDR 问题和随机矩阵理论中所谓的“尖峰模型”进行类比，我们提出了鲁棒的波束形成解决方案，这些解决方案被证明优于经典方法（例如，匹配滤波器和样本矩阵求逆技术），如 以及更稳健的解决方案，例如基于对角加载的方法。 我们方法的关键是优化逆协方差估计器的设计，它应用为 MVDR 应用量身定制的特征值裁剪和收缩函数。 我们提出的 MVDR 解决方案简单、封闭且易于实施。


## 30. [SpaceBeam: LiDAR-Driven One-Shot mmWave Beam Management](https)
- **整理时间：** 2023-3-25
- **出处：** MpbiSys'21
- **关键词：** 
- **摘要：** 毫米波 5G 网络有望实现需要高吞吐量和超低延迟组合的新一代网络应用。 然而，在实践中，由于管理高度定向波束所需的大量开销，毫米波性能对于大量用户的扩展性很差。 我们发现，通过使用 LiDAR 传感器生成的周围环境的带外红外测量，我们可以大大减少或消除这种开销。 为实现这一目标，我们开发了一种光线追踪系统，该系统对红外传感器的噪声和其他伪影具有鲁棒性，创建了一种方法来估计传感器数据的反射强度，最后将此信息应用于多用户光束选择过程。 我们证明了这种方法在室内多用户场景中将波束选择开销减少了 95% 以上，在移动场景中将网络延迟减少了 80% 以上并将吞吐量提高了 2 倍以上。

- **应用场景：** </br> 
    - How do we transform 3D environment data into RF models to achieve one-shot mmWave beam selection in massive high density networks?
    - 我们如何将 3D 环境数据转换为射频模型以在大规模高密度网络中实现一次性毫米波波束选择？

- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_30_fig1.png" alt="image" width ="80%">
    </div>
    

## 29. [FaceSense: Sensing Face Touch with an Ear-worn System](https://www.cs.columbia.edu/~xia/publication/ubicomp21-facesense/ubicomp21-facesense.pdf)
- **整理时间：** 2023-3-25
- **出处：** UbiComp'21
- **关键词：** 面部触摸检测，热生理传感，多模态深度学习。
- **摘要：** 面部触摸是一种无意识的人类习惯。 经常触摸敏感/粘膜面部区域（眼睛、鼻子和嘴巴）会通过将病原体带入体内并传播疾病来增加健康风险。 此外，准确监测面部触摸对于行为干预至关重要。 现有的监控系统仅捕获接近面部的物体，而不是检测实际触摸。 因此，这些系统很容易在人脸附近的手或物体移动时出现误报（例如，拿起电话）。 我们展示了 FaceSense，这是一种耳戴式系统，能够识别实际触摸并将它们区分敏感/粘膜区域与其他面部区域。 按照多模式方法，FaceSense 集成了低分辨率热图像和生理信号。 热传感器感应手靠近时发出的热红外信号，而生理传感器则监测触摸过程中皮肤变形引起的阻抗变化。 处理过的热信号和生理信号被输入深度学习模型 (TouchNet) 以检测触摸并识别触摸的面部区域。 我们使用现成的硬件制作了原型，并在 14 名参与者进行各种日常活动（例如，喝酒、说话）时对他们进行了实验。 结果显示，使用留一用户交叉验证的触摸检测的宏观 F1 分数为 83.4%，使用个性化模型进行触摸区域识别的宏观 F1 分数为 90.1%。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_29_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_29_fig2.png" alt="image" width ="80%">
    </div> 


## 28. [Cross Vision-RF Gait Re-identification with Low-cost RGB-D Cameras and mmWave Radars](https://arxiv.org/pdf/2207.07896.pdf)
- **整理时间：** 2023-3-25
- **出处：** UbiComp'22
- **关键词：** 交叉模态、步态再识别、毫米波传感、镜面反射, ReID
- **Abstract:** Human identification is a key requirement for many applications in everyday life, such as personalized services, automatic surveillance, continuous authentication, and contact tracing during pandemics, etc. This work studies the problem of cross-modal human re-identification (ReID), in response to the regular human movements across camera-allowed regions (e.g., streets) and camera-restricted regions (e.g., offices) deployed with heterogeneous sensors. By leveraging the emerging low-cost RGB-D cameras and mmWave radars, we propose the first-of-its-kind vision-RF system for cross-modal multi-person ReID at the same time. Firstly, to address the fundamental inter-modality discrepancy, we propose a novel signature synthesis algorithm based on the observed specular reflection model of a human body. Secondly, an effective cross-modal deep metric learning model is introduced to deal with interference caused by unsynchronized data across radars and cameras. Through extensive experiments in both indoor and outdoor environments, we demonstrate that our proposed system is able to achieve ~ 92.5% top-1 accuracy and ~ 97.5% top-5 accuracy out of 56 volunteers. We also show that our proposed system is able to robustly reidentify subjects even when multiple subjects are present in the sensors' field of view.

- **摘要：** 人体识别是日常生活中许多应用的关键要求，例如:个性化服务、自动监视、持续身份验证和大流行期间的接触者追踪等。这项工作研究了跨模态人体重新识别（ReID）的问题，在对部署有异构传感器的摄像头允许区域（例如街道）和摄像头限制区域（例如办公室）之间的常规人体运动做出响应。 通过利用新兴的低成本 RGB-D 相机和毫米波雷达，我们提出了首个同时用于跨模态多人 ReID 的视觉 RF 系统。 首先，为了解决基本的模态间差异，我们提出了一种基于观察到的人体镜面反射模型的新型签名合成算法。 其次，引入了一种有效的跨模态深度度量学习模型来处理雷达和相机之间数据不同步造成的干扰。 通过在室内和室外环境中进行的大量实验，我们证明我们提出的系统能够在 56 名志愿者中达到约 92.5% 的 top-1 准确度和约 97.5% 的 top-5 准确度。 我们还表明，即使传感器视野中存在多个主体，我们提出的系统也能够稳健地重新识别主体。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_28_fig2.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_28_fig1.png" alt="image" width ="80%">
    </div> 


## 27. [Two beams are better than one: Towards Reliable and High Throughput mmWave Links](https)
- **整理时间：** 2023-3-25
- **出处：** SigComm'21
- **关键词：** 毫米波、可靠性、吞吐量、模拟波束成形、相控阵、5G NR、多波束、跟踪、阻塞、移动性。
- **摘要：** 具有高吞吐量和高可靠性的毫米波通信有望成为 V2X 和 VR 应用的游戏规则改变者。 然而，毫米波链路因低可靠性而臭名昭著，因为它们经常因阻塞和用户移动而中断。 我们构建了 mmReliable，这是一个可靠的毫米波系统，可实现多波束成形和用户跟踪以处理环境漏洞。 它创建建设性的多波束模式并优化它们的角度、相位和幅度，以最大限度地提高接收器的信号强度。 多波束链路是可靠的，因为与单波束系统相比，它们对少数组成波束的偶尔阻塞具有弹性。 我们在具有 400 MHz 带宽的 28 GHz 测试台和支持 5G NR 波形的 64 元件相控阵上实施 mmReliable。 严格的室内和室外实验表明，mmReliable 实现了接近 100% 的可靠性，与单光束系统相比，吞吐量可靠性产品提高了 2.3 倍。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_27_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_27_fig2.png" alt="image" width ="80%">
    </div> 


----

INFOCOM 2023 毫米波（mmWave）相关9篇

----
## 26. [Universal Targeted Adversarial Attacks Against mmWave-based Human Activity Recognition](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波，人类活动识别，对抗学习，通用目标攻击，黑盒攻击
- **摘要：** 基于毫米波 (mmWave) 技术的人体活动识别 (HAR) 系统近年来得到了发展，因为它们具有更好的隐私保护和增强的传感器分辨率。 随着 HAR 系统部署的不断增长，此类系统的漏洞已经暴露出来。 然而，HAR 对抗性攻击的现有努力仅关注无针对性的攻击。 在本文中，我们提出了第一个通过设计的通用扰动针对基于毫米波的 HAR 的针对性对抗攻击。 开发了一种实用的迭代算法来制作扰动，这些扰动可以很好地概括不同的活动样本，而无需额外的训练开销。 与仅针对特定的基于毫米波的 HAR 模型开发对抗性攻击的现有工作不同，我们通过将目标扩展到两种最常见的基于毫米波的 HAR 模型（即基于体素和基于热图的 HAR）来提高攻击的实用性 楷模）。 此外，我们考虑了一个更具挑战性的黑盒场景，通过知识蒸馏（KD）解决信息不足问题，并通过生成对抗网络（GAN）解决活动样本不足的问题。 我们对针对健身追踪设计的两种不同的基于毫米波的 HAR 模型提出的攻击进行了评估。 评估结果证明了所提出的针对性攻击的有效性、效率和实用性，平均成功率超过 80%。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_26_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_26_fig2.png" alt="image" width ="80%">
    </div> 


## 25. [Rotation Speed Sensing with mmWave Radar](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波感知旋转
- **摘要：** 带有旋转部件的机器在工业系统和我们的日常生活中很普遍。 转速测量是监测机械健康状况的一项重要任务。 以往的转速传感方法受到操作距离有限、对照明的严格要求或对目标物体光反射率的强烈依赖性的限制。 在这项工作中，我们提出了 mRotate，一种实用的基于毫米波雷达的转速传感系统，摆脱了上述所有限制。 具体来说，mRotate将旋转物体反射的目标信号从混合反射信号中分离出来，提取高质量的旋转相关特征，通过定制化的雷达感知模式和算法设计，准确获取旋转速度。 我们在商用毫米波雷达上实施 mRotate，并在实验室环境和用于现场测试的加工车间对其进行广泛评估。 mRotate 在精度测试中实现了 0.24% 的 MAPE，比基准设备（一种流行的商用激光转速计）产生的 MAPE 低 38%。 此外，我们的实验表明，mRotate 可以测量直径仅为 5mm 的主轴，并在远至 2.5m 的感应距离下保持高精度，并同时测量多个物体的旋转速度。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_25_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_25_fig2.png" alt="image" width ="80%">
    </div> 



## 24. [mmEavesdropper: Signal Augmentation-based Directional Eavesdropping with mmWave Radar](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 
- **摘要：** 随着配备扬声器的在线会议的普及，语音隐私安全越来越受到关注，因为窃听扬声器可以快速获取敏感信息。 在本文中，我们提出了 mmEavesdropper，一种基于毫米波的窃听系统，其重点是通过语音恢复的理论模型来增强微振动信号。 特别是，为了增强目标振动的接收信号，我们建议使用波束形成通过抑制其他方向来促进方向增强，并使用 Chirp-Z 变换通过与传统 FFT 相比提高距离分辨率来促进距离增强。 为了增强 IQ 平面中的振动信号，我们建立了一个理论模型来分析失真，并提出了一种基于分段的拟合方法来校准振动信号。 为了增加声音恢复的频谱，我们建议组合多个通道并利用基于编码器-解码器的神经网络来重建语音恢复的频谱。 我们对 mmEavesdropper 进行了大量实验，结果表明 mmEavesdropper 可以达到 93% 的数字和字母识别准确率。 此外，mmEavesdropper 可以重建平均 SNR 为 5dB 和峰值 SNR 为 17dB 的语音。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_24_fig1.png" alt="image" width ="80%">
    </div>
    

## 23. [Safehaul: Risk-Averse Learning for Reliable mmWave Self-Backhauling in 6G Networks](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波通信、集成接入和回程 (IAB)、自回程、无线回程
- **摘要：** 在静态场景中以毫米波频率 (mmWave) 进行无线回传是蜂窝网络中公认的做法。 然而，当今毫米波系统中的高度定向和自适应波束成形为自回程开辟了新的可能性。 利用这一潜力，3GPP 标准化了集成接入和回程 (IAB)，允许同一基站同时服务接入和回程流量。 尽管 IAB 毫米波网络中的资源分配和路径选择更具成本效益和灵活性，但仍是一项艰巨的任务。 迄今为止，之前的工作通过大量经典的优化和学习方法解决了这一挑战，通常优化吞吐量、延迟和公平性等关键性能指标 (KPI)，而很少关注 KPI 的可靠性。 我们提出了 Safehaul，这是一种用于 IAB 毫米波网络的基于学习的风险规避解决方案。 除了优化平均性能外，Safehaul 还通过最小化性能分布尾部的损失来确保可靠性。 我们开发了一种新颖的模拟器，并通过广泛的模拟表明，与基准相比，Safehaul 不仅将延迟减少了高达 43.2%，而且还表现出明显更可靠的性能（例如，实现的延迟差异减少了 71.4%）。

- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_23_fig1.png" alt="image" width ="80%">
    </div> 

## 22. [Argosleep: Monitoring Sleep Posture from Commodity Millimeter-Wave Devices](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 
- **摘要：** 我们提出 Argosleep，这是一种基于毫米波 (mmWave) 无线传感器的睡眠姿势监测系统，可预测人在睡眠期间身体关节的 3D 位置。 Argosleep 利用深度学习模型和人体解剖学特征知识来解决现有毫米波设备中的低分辨率、镜面反射和混叠问题。 Argosleep 通过从数千个现有样本中学习毫米波反射信号与身体姿势之间的关系来构建模型。 由于实际睡眠也涉及突然的翻身，这可能会导致姿势预测错误，因此 Argosleep 设计了一个基于反射信号的状态机，将睡眠状态分为休息或翻身，并仅在休息状态下预测姿势 . 我们使用从 COTS 毫米波设备收集的真实数据对 Argosleep 进行评估，这些数据来自 8 名不同年龄、性别和身高的志愿者，他们表现出不同的睡眠姿势。 我们观察到 Argosleep 准确地识别了翻滚事件并预测了身体关节的 3D 位置，其准确度与现有的基于视觉的系统相当，释放了毫米波系统在隐私非侵入式家庭医疗保健应用中的潜力。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_22_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_22_fig2.png" alt="image" width ="80%">
    </div> 

## 21. [High-speed Machine Learning-enhanced Receiver for Millimeter-Wave Systems](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 机器学习、毫米波、信道估计、物理层、均衡
- **摘要：** ML 是设计无线 PHY 组件的很有前途的工具。 由于这些频率下的硬件设计和信道环境更具挑战性，因此对于毫米波及更高版本尤其有趣。 在本文中，我们没有构建单独的 ML 组件，而是为频率选择信道设计了一个完整的 ML 增强型毫米波接收器。 我们的 ML 接收器使用卷积神经网络联合优化信道估计、均衡、相位校正和解映射器。 我们还表明，对于毫米波系统，信道即使在短时间尺度内也会发生显着变化，需要频繁进行信道测量，而这种情况在移动场景中会加剧。 为了解决这个问题，我们提出了一种新的 ML 信道估计方法，该方法使用可用于通信数据包中每个符号块的保护间隔（不适用于信道测量）来刷新信道状态信息。 据我们所知，我们的 ML 接收器是第一个在一般情况下优于传统接收器的工作，仿真结果显示增益高达 7 dB。 我们还提供了 ML 增强型接收器的首次实验验证，该接收器具有基于 60 GHz FPGA 的测试平台和相控阵天线阵列，这表明在移动场景中吞吐量比基线方案增加了 6 倍。

- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_21_fig1.png" alt="image" width ="80%">
    </div> 

## 20. [MIA: A Transport-Layer Plugin for Immersive Applications in Millimeter Wave Access Networks](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波、沉浸式应用、带宽预测、强化学习、TCP
- **摘要：** 毫米波 (mmWave) 波束的高度定向特性对使用该频谱满足沉浸式应用的通信需求提出了多项挑战。 特别是，毫米波波束容易受到用户移动造成的错位和阻塞的影响。 因此，毫米波信道容易受到质量大幅波动的影响，这反过来会导致基于传输控制协议 (TCP) 的应用程序的端到端性能不成比例地下降。 在本文中，我们提出了一种强化学习 (RL) 集成传输层插件，即基于毫米波的沉浸式代理 (MIA)，用于通过毫米波链路交付沉浸式内容。 MIA 使用 RL 模型根据实时测量预测毫米波链路带宽。 然后，MIA 与 TCP 的拥塞控制方案合作，根据毫米波带宽的预测调整发送速率。 为了评估所提出的 MIA 的有效性，我们使用毫米波增强沉浸式测试台和网络模拟进行实验。 评估结果表明，MIA 在吞吐量和延迟方面显着提高了端到端沉浸式性能。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_20_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_20_fig2.png" alt="image" width ="80%">
    </div> 


## 19. [flexRLM: Flexible Radio Link Monitoring for Multi-User Downlink Millimeter-Wave Networks](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波，多用户网络，无线电链路监控，波束管理
- **摘要：** 为高容量多用户网络开发毫米波 (mm-wave) 的前提是联合执行波束管理，以实现所有用户之间的无缝连接和高效资源共享。 5G-NR 中的波束管理主动监控服务小区上的候选波束对链路 (BPL)，以简单地选择用户的最佳波束，但忽略了多用户资源共享问题，可能导致过载小区的吞吐量严重下降。 我们提出了 flexRLM，一种用于多用户下行链路毫米波网络的基于协调器的灵活无线电链路监控 (RLM) 框架。 flexRLM 允许在服务和其他候选小区上灵活配置受监控的 BPL，并联合考虑链路质量和资源共享进行波束选择。 flexRLM 完全符合 5G-NR 标准，并在非独立模式下使用 LTE 协调器，通过来自周期性下行链路控制同步信号的测量报告不断更新受监控的 BPL。 我们在 ns-3 中实现了 flexRLM，并展示了全栈模拟，以证明 flexRLM 在多用户网络中优于默认 5G-NR RLM 的卓越性能。 我们的结果表明，flexRLM 对受监控 BPL 的持续更新提高了链路质量和稳定性。 通过监控服务小区以外的候选小区上的 BPL，flexRLM 还显着减少了切换决策延迟。 重要的是，flexRLM 的低复杂性协调负载平衡实现了接近单用户基线的每用户吞吐量。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_19_fig1.png" alt="image" width ="80%">
    </div>
    

## 18. [On the Effective Capacity of RIS-enabled mmWave Networks with Outdated CSI](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波智能表面（mmWave RIS）
- **摘要：** 可重构智能表面 (RIS) 具有提高毫米波网络覆盖范围的巨大潜力； 然而，获取支持 RIS 的毫米波网络的完美信道状态信息 (CSI) 具有挑战性且成本高昂。 另一方面，在提供典型系统性能的过时 CSI 存在的情况下，很难找到最佳 RIS 配置。 为此，这项工作旨在通过使用有效容量作为分析工具，为 CSI 的过时性和系统性能之间的权衡提供实用的见解。 我们考虑启用 RIS 的毫米波下行链路，基站在统计服务质量约束下运行。 我们找到了有效容量的封闭形式表达式，其中包含数据包调度的乐观程度以及瞬时和过时 CSI 之间的相关强度。 此外，我们的分析使我们能够找到信号与干扰加噪声比 (SINR) 分布参数的最佳值及其对不同网络场景中有效容量的影响。 仿真结果表明，当已知信道估计已过时时，使用次优 RIS 配置可以获得更好的有效容量。 它使我们能够设计系统参数，以保证更好的性能，同时将与信道估计相关的复杂性和成本保持在最低水平。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_18_fig1.png" alt="image" width ="80%">
    </div>
    

## 17. [mmFlexible: Flexible Directional Frequency Multiplexing for Multi-user mmWave Networks](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波、波束成形、延迟相控阵、频率复用、OFDMA、调度
- **摘要：** 由于执行定向频率复用的不灵活性，现代毫米波系统无法扩展到大量用户。 毫米波信号中的所有频率分量都通过笔形波束向一个方向进行波束成形，无法流式传输到其他用户方向。 我们展示了 mmFlexible，这是一种灵活的毫米波系统，可实现灵活的定向频率复用，允许不同的频率分量使用同一笔形波束在多个任意方向上辐射。 我们做出了两项重要贡献：1. 我们提出了一种称为延迟相控阵的新型毫米波前端架构，它使用可变延迟和可变相位元件来创建所需的频率方向响应。 2. 我们提出了一种新算法来估计延迟相控阵实时操作的延迟和相位值。 我们的前端架构创建了一个抽象，允许任何 OFDMA 调度器像 sub-6 一样灵活地运行，而没有任何固定的方向限制。 我们对室内和室外毫米波信道轨迹的评估显示，吞吐量比传统相控阵架构提高了 1.3 倍，比实时延迟架构提高了 3.9 倍； 同时将最坏情况下的延迟减少 72%。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_17_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_17_fig2.png" alt="image" width ="80%">
    </div> 


## 16. [Realizing Uplink MU-MIMO Communication in mmWave WLANs: Bayesian Optimization and Asynchronous Transmission](https)
- **整理时间：** 2023-3-25
- **出处：** INFOCOM 2023
- **关键词：** 毫米波，MU-MIO，6G，贝叶斯学习，通信相关，硬件设备USRP X310
- **摘要：** 随着移动设备的激增，毫米波 (mmWave) 和 MIMO 技术的结合是满足数据密集型应用的通信需求的自然趋势。 顺应这一趋势，毫米波多用户 MIMO (MU-MIMO) 已被 IEEE 802.11ay 标准化，其下行链路可实现多 Gbps 数据速率。 然而，它的上行链路对应物尚未得到很好的研究，其通往无线局域网 (WLAN) 的途径仍不清楚。 在本文中，我们提出了一种适用于 WLAN 的实用上行链路 MU-MIMO 毫米波通信 (UMMC) 方案。 UMMC 有两个关键组件：i) 用于在多个定向天线上进行联合波束搜索的高效贝叶斯优化 (BayOpt) 框架，以及 ii) 可以解码来自多个用户设备的异步数据包的新型 MU-MIMO 检测器。 我们在毫米波测试台上构建了 UMMC 原型，并通过空中实验和大量模拟相结合的方式评估了其性能。 实验和仿真结果证实了 UMMC 在实际网络设置中的效率。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_16_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_16_fig2.png" alt="image" width ="80%">
    </div> 


------

## 15. [mmPose-NLP: A Natural Language Processing Approach to Precise Skeletal Pose Estimation using mmWave Radars](https://arxiv.org/pdf/2107.10327.pdf)
- **整理时间：** 2023-3-25
- **出处：** IEEE Transactions on Neural Networks and Learning Systems ( Early Access )
- **关键词：** 毫米波雷达、姿态估计、Seq2Seq、骨骼姿态、NLP、骨骼关键点、GRU、点云
- **摘要：** 在本文中，我们介绍了 mmPose-NLP，这是一种使用毫米波 (mmWave) 雷达数据的新型自然语言处理 (NLP) 启发序列到序列 (Seq2Seq) 骨架关键点估计器。 据作者所知，这是第一种仅使用毫米波雷达数据即可精确估计多达 25 个骨骼关键点的方法。 骨骼姿势估计在自动驾驶汽车、交通监控、患者监控、步态分析、国防安全取证等多种应用中至关重要，并有助于预防性和可操作性的决策制定。 与传统使用的光学传感器相比，将毫米波雷达用于此任务具有多个优势，主要是它对场景照明和恶劣天气条件的操作鲁棒性，在这些条件下光学传感器性能会显着降低。 毫米波雷达点云 (PCL) 数据首先被体素化（类似于 NLP 中的标记化），体素化雷达数据的 N 帧（类似于 NLP 中的文本段落）受到建议的 mmPose-NLP 架构的影响，其中体素 预测了 25 个骨骼关键点的索引（类似于 NLP 中的关键字提取）。 使用标记化过程中使用的体素字典将体素索引转换回现实世界的 3-D 坐标。 平均绝对误差 (MAE) 指标用于衡量拟议系统相对于地面实况的准确性，拟议的 mmPose-NLP 在深度、水平和垂直轴上提供 <3 cm 的定位误差。 对于 N = {1,2,..,10}，还研究了输入帧数与性能/精度的影响。 本文介绍了全面的方法、结果、讨论和局限性。 所有源代码和结果都在 GitHub 上提供，用于在使用毫米波雷达的骨骼关键点估计这个关键但新兴的领域进一步研究和开发。

- **系统框架：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_15_fig1.png" alt="image" width ="80%">
    </div>
    
- **实验结果：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_15_fig2.png" alt="image" width ="80%">
    </div> 


## 14. [WaveSpy: Remote and Through-wall Screen Attack via mmWave Sensing](https://engineering.purdue.edu/~lusu/papers/S&P2020.pdf)
- **[PPT(YouTube)](https://www.youtube.com/watch?v=J7YrEoHU55E)**
- **整理时间：** 2023-3-25
- **出处：** 2020 IEEE Symposium on Security and Privacy (SP)
- **关键词：** 窃听，毫米波，窗墙屏幕
- **摘要：** 数字屏幕，例如液晶显示器 (LCD)，容易受到攻击（例如“肩窥”），可以绕过安全保护服务（例如防火墙）窃取目标受害者的机密信息。 减轻这些威胁的传统做法是隔离。 一个没有可访问性、邻近性和视线的隔离区，似乎将个人设备带到了一个真正安全的地方。在本文中，我们重新审视这个历史话题，重新审视隔离场景下屏幕攻击的安全风险 上文提到的。 具体来说，我们通过使用低成本射频传感器的液晶向列状态估计，识别并验证了一种新的实用的屏幕内容侧信道攻击。 通过利用屏幕内容与显示器中液晶阵列状态之间的关系，我们开发了 WaveSpy，一种端到端的便携式穿墙屏幕攻击系统。 WaveSpy 包含一个低成本、节能且重量轻的毫米波 (mmWave) 探头，即使将受害者的屏幕放在 一个孤立的区域。 我们集中评估了 WaveSpy 在屏幕攻击中的性能和实用性，包括现代电子设备 30 个数字屏幕上的 100 多种不同类型的内容。 WaveSpy 在真实场景下的屏幕内容类型识别准确率达到 99%，Top-3 敏感信息检索成功率达到 87.77%。 此外，我们讨论了几种潜在的防御机制来减轻类似于 WaveSpy 的屏幕窃听。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_14_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_14_fig2.png" alt="image" width ="80%">
    </div> 


## 13. [MILLIEAR: Millimeter-wave Acoustic Eavesdropping with Unconstrained Vocabulary](https)
- **阅读时间：** 2023-3-24
- **出处：** INFOCOM'22
- **关键词：** 毫米波语音窃听，mmWave, 穿过玻璃窃听扬声器的语音信号
- **摘要：** 随着声学通信系统在家庭和办公室中变得越来越普遍，窃听会带来重大的安全和隐私风险。 当前的声学窃听方法要么由于使用低于 6 GHz 的频率而提供低分辨率，仅适用于使用分类的有限单词，要么由于使用光学传感器而无法穿墙工作。 在本文中，我们介绍了 MILLIEAR，这是一种毫米波声学窃听系统，它利用毫米波 FMCW 测距的高分辨率和生成式机器学习模型，不仅可以提取振动，还可以重建音频。 MILLIEAR 将说话人振动估计与条件生成对抗网络相结合，以使用不受约束的词汇进行窃听。 我们使用部署在不同场景和设置中的现成毫米波雷达来实施和评估 MIL-LIEAR。 我们发现，即使在不同的距离、角度和不同绝缘体材料的墙壁上，它也能准确地重建音频。 我们的主观和客观评估表明，重建后的音频与原始音频具有很强的相似性。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_13_fig1.png" alt="image" width ="80%">
    </div>
    

## 12. [Spatially Sparse Precoding in Millimeter Wave MIMO Systems](https)
- **阅读时间：** 2023-3-24
- **出处：** ICC'2013
- **关键词：** 毫米波MIMO系统和信道建模
- **摘要：** 毫米波 (mmWave) 信号的路径损耗比目前大多数无线应用中使用的微波信号多几个数量级。 因此，毫米波系统必须利用波长缩短的大型天线阵列，以通过波束成形增益来对抗路径损耗。 具有多个数据流的波束成形（称为预编码）可用于进一步提高毫米波频谱效率。 在传统的多天线系统中，波束成形和预编码都是在基带上以数字方式完成的。 然而，毫米波系统中混合信号设备的高成本和功耗使得射频领域的模拟处理更具吸引力。 这种硬件限制限制了实用毫米波收发器可以应用的一组可行的预编码器和组合器。 在本文中，我们考虑在具有大型天线阵列的毫米波系统中进行发射预编码和接收器组合。 我们利用毫米波信道的空间结构将预编码/组合问题表述为稀疏重建问题。 使用基追踪原理，我们开发了准确近似最优无约束预编码器和组合器的算法，以便它们可以在低成本 RF 硬件中实现。 我们展示了所提出算法性能的数值结果，并表明它们允许毫米波系统接近其不受约束的性能极限，即使在考虑收发器硬件约束的情况下也是如此。

- **系统硬件框图：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_12_fig1.png" alt="image" width ="80%">
    </div>
    

## 11. [Wavesdropper: Through-wallWord Detection of Human Speech via Commercial mmWave Devices](https://dl.acm.org/doi/10.1145/3534592)
- **阅读时间：** 2023-3-24
- **出处：** UbiComp'22
- **关键词：** 文字检测，毫米波感知（mmWave），穿墙
- **摘要：** 大多数现有的窃听攻击利用传播声波进行语音检索。 然而，隔音材料广泛应用于对语音敏感的场景（例如会议室）。 在本文中，我们揭示了受隔离房间保护的人类语音可能会受到便携式和商用现成毫米波设备的影响。 为了实现这一目标，我们开发了 Wavesdropper，这是一种单词检测系统，它利用毫米波探头来感知目标说话者的喉咙振动并在受阻条件下恢复语音内容。我们提出了一种基于 CEEMD 的方法来抑制动态杂波（例如，人体运动）和基于小波的处理方法从混合信号中提取微妙的声音振动信息。 为了从与声音振动相关的毫米波信号中恢复语音内容，我们设计了一个神经网络来推断语音内容。 此外，我们使用多个（两个）探针探索了对话中的单词检测，并揭示了对手可以仅使用一个毫米波设备同时检测多人的单词。 我们进行了广泛的实验来评估超过 60,000 个发音的系统性能。 实验结果表明，Wavesdropper 在 23 名志愿者身上识别 57 个词的准确率可以达到 91.3%。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_11_fig1.png" alt="image" width ="80%">
    </div>
    
- **系统框架：**

    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_11_fig2.png" alt="image" width ="80%">
    </div> 
    
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_11_fig3.png" alt="image" width ="80%">
    </div> 

## 10. [RF-ECG: Heart Rate Variability Assessment Based on COTS RFID Tag Array](https://personal.stevens.edu/~ychen6/papers/RF-ECG-%20Heart%20Rate%20Variability%20Assessment%20Based%20on%20COTS%20RFID%20Tag%20Array.pdf)
- **阅读时间：** 2023-3-24
- **出处：** UbiComp’18
- **关键词：** RFID 测心跳
- **摘要：** 心率变异性(Heart Rate Variability, HRV)作为循环功能自主调节的重要指标，广泛应用于全身健康评估。 除了以有线方式使用专用设备（例如 ECG）之外，当前的方法通过使用精度低和电池寿命有限的可穿戴设备或应用无线技术（例如 FMCW）来寻找无处不在的方式，这通常 利用专用设备（例如 USRP）进行测量。 为了解决这些问题，我们提出了基于商用现成 (COTS) RFID 的 RF-ECG，这是一种无线方法，通过附着在衣服胸部区域的 RFID 标签阵列来感应人体心跳。 特别是，当 RFID 阅读器连续询问标签阵列时，标签阵列会捕获两个主要效果： 反射效果代表从心跳引起的心脏运动反射的 RF 信号； 移动效果表示由于呼吸引起的胸部运动引起的标签运动。 为了从嘈杂的 RF 信号中提取反射信号，我们开发了一种机制来捕获由移动效应引起的标签阵列的 RF 信号变化，旨在消除与呼吸相关的信号。 为了根据反射信号估计 HRV，我们提出了一个信号反射模型来描述来自标签阵列的 RF 信号变化与与心跳相关的反射效应之间的关系。 开发了一种融合技术来组合来自标签阵列的多个反射信号，以准确估计 HRV。 对 15 名志愿者进行的实验表明，RF-ECG 可以实现心跳间隔 (IBI) 的 3% 的中值误差，这与现有的有线技术相当。

- **应用场景：** </br> 
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_10_fig1.png" alt="image" width ="80%">
    </div>


## 9. [A novel beamforming technique using mmWave antenna arrays for 5G wireless communication networks](https://www.sciencedirect.com/science/article/abs/pii/S105120042300012X)
- **阅读时间：** 2023-3-24
- **出处：** Digital Signal Processing,2023
- **关键词：** 
- **摘要：** 毫米波 (mmWave) 多输入多输出 (MIMO) 和波束成形技术很可能是 5G 及更高版本 (5G-B) 无线通信系统的组成部分和关键推动因素。 从这个角度来看，这份手稿提出了一种适用于 5G 应用的高效数字波束成形技术。 建议的方法是基于可靠的采样技术制定的，该技术可以有效地对干扰加噪声协方差矩阵 (IPNCM) 进行采样以构建有效的投影矩阵 (PM)。 因此，所提出的技术被命名为干扰加噪声 PM (IPNPM) 波束形成器。 接下来，使用 CST 微波工作室设计了一个紧凑型矩形微带天线，其工作频率为 49.3 GHz，潜在带宽为 1.7 GHz。 设计的天线随后用于模拟代表典型 5G 基站的 32 元均匀线性阵列 (ULA)。 然后，建模的 ULA 的元素被手动输入从建议的波束形成器生成的复数权重，以分别向所需和不需要的位置产生高功率波束和深度空值。 为了进一步提高波束形成器在最小化不需要区域内的辐射功率方面的性能，开发了迭代旁瓣电平 (SLL) 抑制技术并将其与所提出的波束形成器集成。 进行的理论分析证明，IPNPM 波束形成器比众所周知的波束形成方法需要更少的算术运算。 为了揭示所提出技术的优势，绘制了基于所提出波束形成器的阵列辐射方向图，并将其与三种广泛使用的方法的辐射方向图进行了比较。 还进行了密集的蒙特卡罗模拟，其中系统地将 IPNPM 波束形成器性能与基于输出信号与干扰加噪声比 (SINR) 标准的流行方法进行了比较。 取得的结果表明，所提出的方法在生成更深的空值、增强的输出 SINR 和更短的执行时间方面优于并超越了竞争对手的算法。 还表明，与现有的 SLL 减少技术不同，新开发的 SLL 抑制器在几次迭代后将所提出的波束形成器的 SLL 减少到预定义的阈值（即 -24 dB）。


## 8. [Multi-Resolution Codebook and Adaptive Beamforming Sequence Design for Millimeter Wave Beam Alignment](https://ieeexplore.ieee.org/abstract/document/7947209#full-text-header)
- **阅读时间：** 2023-3-24
- **出处：** IEEE Transactions on Wireless Communications ( Volume: 16, Issue: 9, September 2017)
- **关键词：** 
- **摘要：** 毫米波 (mm-wave) 通信预计将广泛部署在第五代 (5G) 无线网络中，因为在毫米波频率上有大量带宽可供许可和非许可使用。 为了克服在毫米波段观察到的较高路径损耗，大多数先前的工作都集中在在大规模多输入多输出系统中使用模拟和/或混合波束形成技术设计定向波束形成。 在实际系统中从高度定向波束成形中获得潜在收益取决于足够的信道估计精度水平，其中由于使用高分辨率窄波束探测所有方向所需的大量训练开销，信道估计问题变得更具挑战性。 在本文中，我们考虑多分辨率波束形成序列的设计，使系统能够快速搜索出单路径信道的主导信道方向。 由此产生的设计生成了一个多级波束成形序列，该序列在最小化训练开销和最大化波束成形增益之间取得平衡，其中自适应地选择多级波束成形向量的子集以在受限时间内最大化平均数据速率。 我们提出了一种利用巴特勒矩阵（即广义离散傅里叶变换矩阵）设计分层多分辨率码本的有效方法。 数值结果表明了所提算法的有效性。

- **关注点：**



## 7. [Low-Complexity Accurate Mmwave Positioning for Single-Antenna Users Based on Angle-of-Departure and Adaptive Beamforming](https://ieeexplore.ieee.org/abstract/document/9053493)
- **阅读时间：** 2023-3-24
- **出处：**  ICASSP 2020 - 2020 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)
- **关键词：** 
- **摘要：** 解决了使用下行链路传输配备单天线接收器的移动用户的位置估计问题。 考虑到现实的功率预算，根据可实现的理论性能（Cramér-Rao 边界）分析了与经典 MIMO 和上行链路方案相比这种设置的优势。 基于此分析，提出了一种具有改进的定位性能的低复杂度两步算法，该算法首先执行（粗略的）偏离角估计，然后对下行链路信号进行预编码以向用户方向引入波束成形。 结果表明，即使在系统中存在多个用户的情况下，下行链路中的位置估计可能比上行链路中的位置估计准确得多。  


## 6. [Deep Learning-based Adaptive Beamforming for mmWave Wireless Body Area Network（PASS）](https://ieeexplore.ieee.org/document/9322515)
- **阅读时间：** 2023-3-24
- **出处：** GLOBECOM 2020 - 2020 IEEE Global Communications Conference
- **关键词：** 
- **摘要：** 人工智能（AI）正在成为电信行业的主流。 随着 5G 网络中毫米波的使用，在无线体域网 (WBAN) 应用中将波束成形技术用于体上传感器变得可行。 因此，需要开发可优化 WBAN 网络性能的波束成形算法和可用于算法训练、测试和基准测试的真实数据集。 因此，我们提出了一种用于毫米波 WBAN 的数据集生成方法，该方法利用计算机视觉和基于自适应深度学习的算法来优化毫米波 WBAN 波束成形的性能。 提出了两个主要想法：首先，从视频中的 3D 人体姿势估计中收集人体姿势，并采用生成对抗网络 (GAN) 生成更逼真的姿势； 其次，GAN 旨在使用前一组方向作为输入来预测下一个波束形成方向。 借助可用的标记人体姿势视频，我们生成的 WBAN 数据集为波束形成算法的训练、测试和基准测试提供了足够数量的样本。 此外，所提出的自适应波束形成算法不需要任何侵入式数据收集方法。 我们的数值研究显示了我们提出的方法的优势。


## 5. [Adaptive Codebook-Based Channel Estimation in OFDM-Aided Hybrid Beamforming mmWave Systems](https://ieeexplore.ieee.org/document/9896151)
- **阅读时间：** 2023-3-24
- **出处：** IEEE Open Journal of the Communications Society, 2022
- **关键词：** 
- **摘要：** 为了降低毫米波收发器的硬件复杂性和成本，已经开发了混合波束成形技术，它依赖于接收器和/或发射器可用的信道状态信息 (CSI)。 在毫米波信道估计中，基于压缩感知（CS）的算法（如正交匹配追踪（OMP））已被广泛研究，以利用毫米波信道的稀疏特性。 具体而言，OMP 辅助自适应码本信道估计具有降低实现复杂度的优点，但在低信噪比 (SNR) 情况下表现不理想。 为了解决这个问题，在本文中，我们为正交频分复用 (OFDM) 毫米波系统开发了一种改进的自适应码本信道估计算法，该算法通过利用多载波信号进行联合决策来提高估计性能。 我们的研究表明，所提出的信道估计能够显着提高低 SNR 下的估计精度，同时具有较低的实现复杂度。


## 4. [Wideband Cell-Free mmWave Massive MIMO-OFDM: Beam Squint-Aware Channel Covariance-Based Hybrid Beamforming](https://www.researchgate.net/publication/356948548_Wideband_Cell-Free_mmWave_Massive_MIMO-OFDM_Beam_Squint-aware_Channel_Covariance-based_Hybrid_Beamforming)
- **阅读时间：** 2023-3-24
- **出处：** IEEE Transactions on Wireless Communications ( Volume: 21, Issue: 7, July 2022)
- **关键词：** 
- **摘要：** 本文考虑了用于宽带无细胞毫米波 (cell-free mmWave) 大规模多输入多输出 (MIMO)-正交频分复用 (OFDM) 系统的基于波束斜视感知信道协方差的混合波束形成器的设计。 基于不同的波束斜视意识假设，提出了基于单移相器和双移相器的模拟射频 (RF) 预编码器/组合器策略。 数字预编码/组合阶段是使用集中式设计实现的，最大限度地提高了信号与干扰加噪声比 (SINR) 并依赖于时分双工 (TDD) 支持的上行链路 (UL)/下行链路 (DL) 对偶性 协议和使用相移感知最小均方误差 (MMSE) 或相移未知线性 MMSE (LMMSE) 信道估计器。 通过在不同场景下进行广泛的数值模拟，评估了所提出的波束斜视感知混合波束形成策略的性能。 数值结果表明，波束倾斜感知设计优于波束倾斜未感知策略，特别是在典型的宽带无小区毫米波大规模 MIMO-OFDM 场景中，其中结合了非常高的载波频率、大系统带宽和大规模天线 阵列导致空间宽带效应。



## 3. [Opportunistic Hybrid Beamforming Based on Adaptive Perturbation for mmWave Multi-User MIMO Systems](https://ieeexplore.ieee.org/document/9120703)
- **阅读时间：** 2023-3-24 
- **出处：** 2020 IEEE Wireless Communications and Networking Conference (WCNC)
- **关键词：** 
- **摘要：** 在本文中，我们提出了一种用于时间相关毫米波 (mmWave) 信道的自适应扰动辅助机会混合波束形成 (AP-OHBF) 方案。 基本思想是，所提出的方案扰动信道参数以仅基于信号干扰加噪声比 (SINR) 信息来跟踪信道处于有利条件的调度移动台 (MS) 的信道 的MS。 BS利用这些参数生成预编码器，并采用成功的扰动进行数据传输，从而实现性能提升。 相反，如果扰动导致性能下降，则将其丢弃，而使用与内存中最知名参数对应的预编码器。



## 2. [High-Dimensional MVDR Beamforming: Optimized Solutions Based on Spiked Random Matrix Models](https://hal.science/hal-01957672/document)
- **阅读时间：** 2023-3-24
- **出处：** IEEE Transactions on Signal Processing ( Volume: 66, Issue: 7, 01 April 2018)
- **关键词：** MVDR算法
- **摘要：** 最小方差无失真响应 (MVDR) 波束成形（或 Capon 波束成形）是最流行的自适应阵列处理策略之一，因为它能够在消除干扰的同时提供抗噪能力。 这种波束形成器的一个实际挑战是它涉及接收信号的逆协方差矩阵，必须根据数据进行估计。 在现代高维应用中，众所周知，经典估计器会受到采样噪声的严重影响，从而影响波束形成器的性能。 在这里，我们提出了一种适用于高维设置的 MVDR 波束形成新方法。 特别是，通过与 MVDR 问题和随机矩阵理论中所谓的“尖峰模型”进行类比，我们提出了鲁棒的波束形成解决方案，这些解决方案被证明优于经典方法（例如，匹配滤波器和样本矩阵求逆技术），如 以及更稳健的解决方案，例如基于对角加载的方法。 我们方法的关键是优化逆协方差估计器的设计，它应用为 MVDR 应用量身定制的特征值裁剪和收缩函数。 我们提出的 MVDR 解决方案简单、封闭且易于实施。



## 1. [Adaptive Beamforming Design for mmWave RIS-Aided Joint Localization and Communication](https://arxiv.org/pdf/1911.02813.pdf)
- **阅读时间：** 2023-2-16
- **出处：** 2020 IEEE Wireless Communications and Networking Conference Workshops (WCNCW)
- **关键词：** 智能表面，自适应beamforming，
- **摘要：** 可重构智能表面(RIS)的概念被提出来改变电磁波的传播，例如反射、衍射和折射。 为实现这一目标，需要优化离散 RIS 单元的相位值。 在本文中，我们考虑了用于精确定位和高数据速率传输的RIS辅助毫米波(mmWave)多输入多输出(MIMO)系统。 **我们提出了一种基于分层码本和来自MS(Mobile Station)反馈的自适应移相器设计。(We propose an adaptive phase shifter design based on hierarchical codebooks and feedback from the mobile station (MS).)** 该方案的好处在于RIS不需要部署任何有源传感器和基带处理单元。 在移相器的更新过程中，MS处的组合向量被顺序细化。 仿真结果表明，所提出的算法在定位精度和数据速率方面均优于随机相位设计方案。 此外，即使在低信噪比状态下，性能也收敛于穷举搜索方案的性能。
- **系统框架：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/P2023_1_fig2.png" alt="image" width ="80%">
    </div> 

