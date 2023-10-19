<!--
 * @Author: fanlong
 * @Date: 2023-02-25 14:56:59
 * @LastEditors: fanlong
 * @LastEditTime: 2023-06-11 11:37:02
 * @FilePath: \01_paperNote-nju\Weekly_Report_Paperlist_2023.md
 * @Description: 
 * 
 * @github: https://github.com/fanl0228
 * @Email: fanl@smail.nju.edu.cn
 * Copyright (c) 2023 by fanlong/Nanjing University, All Rights Reserved. 
-->

# 2023-06-09

## 1. CEVAS：Towards Cloud-Edge Collaborative Online Video Analytics with Fine-Grained Serverless Pipelines 
- MMSys'21
- 摘要：
- 系统框架：
<div style="text-align:center">
    <img src="imgs/WRP2023_6_9.fig1.png", width="80%">
</div>

## 2. RT-mDL: Supporting Real-Time Mixed Deep Learning Tasks on Edge Platforms
- Sensys'21


## 3. Batch Adaptative Streaming for Video Analytics
- Infocom'22



# 2023-03-03 [Papers](https://box.nju.edu.cn/library/d0b874f1-ceda-4488-9318-7a487007e8a5/01_Papers/%E7%BB%84%E4%BC%9A/2023-03-03)

## 1. InFi: End-to-end Learnable Input Filter for Resource-efficient Mobile-centric Inference （MobiCom'22）
- MobiCom‘22，中科大
- [Code](https://github.com/yuanmu97/infi)
- [PDF](https://yuanmu97.github.io/preprint/InFi_MobiCom22.pdf)
- 摘要：以移动为中心的人工智能应用对模型推理的资源效率提出了很高的要求。 输入过滤是一种很有前途的方法，可以消除输入中的冗余，从而降低推理成本。 之前的努力已经为许多应用程序量身定制了有效的解决方案，但仍有两个基本问题没有得到解答：(1) 推理工作负载的理论过滤性以指导输入过滤技术的应用，从而避免资源受限的移动应用程序的试错成本 ; (2) 特征嵌入的鲁棒可辨别性允许输入过滤对不同的推理任务和输入内容广泛有效。 为了回答这些问题，我们首先提供输入过滤问题的通用形式化，并从理论上比较推理模型及其输入过滤器的假设复杂性，以了解应用输入过滤的优化潜力。 然后我们提出了第一个端到端可学习的输入过滤框架，它涵盖了大多数最先进的方法，并在具有强大可辨别性的特征嵌入方面超越了它们。 基于我们的框架，我们设计并实现了一个支持六种输入模式的输入过滤系统 InFi。 InFi 是第一个支持文本和传感器信号输入以及资源贫乏的移动系统广泛采用的模型分区部署的公司。 综合评估证实了我们的理论结果，并表明 InFi 由于其通用性和端到端的可学习性，在适用性、准确性和效率方面优于强基线。 对于移动平台上的视频分析应用程序，InFi 可以实现 8.5 倍的吞吐量并节省 95% 的带宽，同时保持超过 90% 的准确度。

- 系统框架：
    <div style="text-align:center">
        <img src="imgs/WRP2023_3_3.fig1.png", width="80%">
    </div>

- 应用部署场景：
    <div style="text-align:center">
        <img src="imgs/WRP2023_3_3.fig2.png", width="80%">
    </div>


## 2. Room-scale Hand Gesture Recognition Using Smart Speakers （SenSys'22）
- senSys'22
- 摘要：由于其细粒度的传感粒度以及在智能手机等消费级电子设备中广泛使用的麦克风和扬声器，声学信号最近被用于非接触式手势识别。 然而，非常有限的感应范围将声学感应限制在用户与近距离设备交互的应用场景中。 在本文中，我们提高了声学传感的范围，并论证了使用商品智能扬声器实现房间规模手势识别的可行性。 我们开发了一系列新颖的信号处理技术，并在两个具有不同数量麦克风的商用智能扬声器原型上实现了我们的系统。 在三个不同的环境中进行了广泛的评估，从 16 名参与者那里收集了 1440 个手势。 实验结果表明，我们的系统可以将传感范围从1 m 显着增加到4--5 m。 在用户距离智能音箱4m且存在强干扰的挑战性场景下，实现的手势识别准确率仍然高于90%。
- 
    <div style="text-align:center">
        <img src="imgs/WRP2023_3_3.fig3.png", width="80%">
    </div>


## 3. Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution 
- ICLR’22
- 时间序列（反）归一化 RevIN
- [Code](https://github.com/ts-kim/RevIN)
- 摘要: 均值和方差等统计属性在时间序列中经常随时间变化，即时间序列数据存在分布偏移问题。 时间分布的这种变化是阻碍准确时间序列预测的主要挑战之一。 为了解决这个问题，我们提出了一种简单而有效的归一化方法，称为可逆实例归一化（RevIN），这是一种具有可学习仿射变换的普遍适用的归一化和非归一化方法。 所提出的方法采用对称结构来删除和恢复时间序列实例的统计信息，从而显着提高时间序列预测的性能，如图 1 所示。我们通过广泛的定量和定性分析证明了 RevIN 的有效性 在各种真实世界的数据集上，解决分布转移问题。
    <div style="text-align:center">
        <img src="imgs/WRP2023_3_3.fig5.png", width="80%">
    </div>

- Overview：文章中认为，时序预测模型具有和其它DNN一样的性质，即对于数据输入的分布敏感。几乎所有的DNN，都是在尝试从某个数据分布中找出与之对应的值或分布，因此BN，LN这种归一化层能够让训练效果变得更好（个人以为是更容易使模型收敛）。时序中输入分布问题在于，每一个时间戳的输入，都和上下文有关系，但是又可以看作和上下文的分布都不同，文章中采用偏移的说法。目前的Informer，N-Beats等都没有做这方面的工作，因此文章在研究后提出了RevIN：可逆实例归一化，用来在时序数据上平稳输入的分布。
    <div style="text-align:center">
        <img src="imgs/WRP2023_3_3.fig4.png", width="80%">
    </div>


# 2023-02-24 [Papers](https://box.nju.edu.cn/library/d0b874f1-ceda-4488-9318-7a487007e8a5/01_Papers/%E7%BB%84%E4%BC%9A/2023-02-24)

## 1. Mobi2Sense: Empowering Wireless Sensing with Mobility
- Mobicom'22
- [PDF](https://dl.acm.org/doi/10.1145/3495243.3560518)
- 设备移动的无线感知（UWB）
- 摘要：除了传统的通信功能外，无线信号最近也被积极地用于传感目的。 然而，现有无线传感的一个缺失组件是在设备运动下进行传感。 这是具有挑战性的，因为设备运动很容易压倒目标运动，例如用于呼吸感应的胸部位移。 本文朝着将设备移动性纳入无线传感生态系统的方向迈出了第一步。 由于近年来超宽带（UWB）芯片的小型化和低成本化，我们提出将超宽带传感的准确性与移动性相结合，以支持真正无处不在的无线传感。 我们提出了 Mobi2Sense，一种支持设备运动感应的系统设计。 我们提出了新颖的信号处理方案，以消除设备运动对使用商用 UWB 硬件的传感和原型 Mobi2Sense 的影响。 实际应用表明，即使存在设备运动，细粒度的 Mobi2Sense 也能够捕捉细微的目标运动，以高精度“听到”音乐、“看到”人类呼吸和“识别”多目标手势。

- 感知原理：
    <div style="text-align:center">
        <img src="imgs/WRP2023_2_24.fig1.png", width="80%">
    </div>


## 2. Experience: Practical Problems for Acoustic Sensing
- MobiCom'22
- 摘要：声学传感显示出巨大的潜力，可以将人们每天与之交互的数十亿消费级电子设备转变为无处不在的传感平台。 在本文中，我们分享了在开发和部署声学传感系统以供实际使用的过程中的经验和发现。 我们确定了研究界未关注的多个实际问题，并提出了相应的解决方案。 挑战包括：（i）存在由声学感应引起的烦人的可听声音泄漏； (ii) 声学感应实际影响音乐播放和语音通话； (iii) 声学感应消耗大量电力，降低电池寿命； (iv) 现实世界的设备移动性可能会导致声学传感失败。 我们希望分享的经验不仅有利于传感算法的未来发展，也有利于硬件设计，推动声学传感在现实生活中更进一步。

- 实际问题1（声音泄露）：麦克风超声波谐波产生影响
    <div style="text-align:center">
        <img src="imgs/WRP2023_2_24.fig2.png", width="80%">
    </div>

- 实际问题2（传感对音乐播放/语音通话的负面影响）
    <div style="text-align:center">
        <img src="imgs/WRP2023_2_24.fig3.png", width="80%">
    </div>

- 实际问题3（感知功耗浪费）


- 实际问题4（设备移动性产生的有害影响）
    <div style="text-align:center">
        <img src="imgs/WRP2023_2_24.fig4.png", width="80%">
    </div>


## 3. IF-ConvTransformer: A Framework for Human Activity Recognition Using IMU Fusion and ConvTransformer
- Ubicomp'22
- [PDF](https://dl.acm.org/doi/10.1145/3534584)
- 摘要：基于传感器的人类活动识别 (HAR) 的最新进展利用深度混合网络来提高性能。 这些混合模型结合了卷积神经网络 (CNN) 和递归神经网络 (RNN)，以利用它们的互补优势，并取得了令人印象深刻的结果。 然而，这些模型没有充分考虑 HAR 中不同传感器的作用和关联，导致多模态融合不足。 此外，HAR 中常用的 RNN 存在“遗忘”缺陷，这增加了捕获长期信息的困难。 为了解决这些问题，本文提出了一种由惯性测量单元 (IMU) 融合块和应用的 ConvTransformer 子网组成的 HAR 框架。 受互补滤波器的启发，我们的 IMU 融合块根据物理关系对常用传感器进行多模态融合。 因此，可以更有效地聚合不同模态的特征。 然后，将提取的特征馈送到应用的 ConvTransformer 子网中进行分类。 得益于其卷积子网和自注意力层，ConvTransformer 可以更好地捕获局部特征并构建长期依赖关系。 在八个基准数据集上进行的大量实验证明了我们框架的卓越性能。 源代码将很快发布。

- Overview
    <div style="text-align:center">
        <img src="imgs/WRP2023_2_24.fig5.png", width="80%">
    </div>


