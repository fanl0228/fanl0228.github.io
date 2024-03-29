---
title: "Intensive Reading [Year 2023]"
excerpt: This note details the application scenario, paper contribution, system framework, experimental setup, etc.
toc: true
---


## [Papaers path](https://box.nju.edu.cn/library/d0b874f1-ceda-4488-9318-7a487007e8a5/01_%E9%98%85%E8%AF%BB%E8%AE%BA%E6%96%87/2023_Intensive_Reading)


## 5. [IndexPen: Two-Finger Text Input with Millimeter-Wave Radar](https://www.researchgate.net/publication/361826003_IndexPen_Two-Finger_Text_Input_with_Millimeter-Wave_Radar)
- **阅读时间：** 2023-3-12

- **出处：** UbiComp'22

- **关键词：** 微手势识别；毫米波FMCW雷达； 微手势感应； 空中手势； 深度学习； 文字输入； 光标交互

- **Abstract：** In this paper, we introduce IndexPen, a novel interaction technique for text input through two-finger in-air micro-gestures, enabling touch-free, effortless, tracking-based interaction, designed to mirror real-world writing. Our system is based on millimeter-wave radar sensing, and does not require instrumentation on the user. IndexPen can successfully identify 30 distinct gestures, representing the letters A-Z, as well as Space, Backspace, Enter, and a special Activation gesture to prevent unintentional input. Additionally, we include a noise class to differentiate gesture and non-gesture noise. We present our system design, including the radio frequency (RF) processing pipeline, classification model, and real-time detection algorithms. We further demonstrate our proof-of-concept system with data collected over ten days with five participants yielding 95.89% cross-validation accuracy on 31 classes (including noise). Moreover, we explore the learnability and adaptability of our system for real-world text input with 16 participants who are first-time users to IndexPen over five sessions. After each session, the pre-trained model from the previous five-user study is calibrated on the data collected so far for a new user through transfer learning. The F-1 score showed an average increase of 9.14% per session with the calibration, reaching an average of 88.3% on the last session across the 16 users. Meanwhile, we show that the users can type sentences with IndexPen at 86.2% accuracy, measured by string similarity. This work builds a foundation and vision for future interaction interfaces that could be enabled with this paradigm.

- **摘要：** 在本文中，我们介绍了 IndexPen，这是一种通过双指空中微手势进行文本输入的新颖交互技术，可实现免触摸、轻松、基于跟踪的交互，旨在反映真实世界的书写。 我们的系统基于毫米波雷达传感，不需要用户使用仪器。 IndexPen 可以成功识别 30 种不同的手势，代表字母 A-Z，以及 Space、Backspace、Enter 和一种特殊的 Activation 手势，以防止无意输入。 此外，我们还包括一个噪声类来区分手势和非手势噪声。 我们展示了我们的系统设计，包括射频 (RF) 处理管道、分类模型和实时检测算法。 我们进一步展示了我们的概念验证系统，其中收集了十天的数据，五名参与者在 31 个类别（包括噪音）上产生了 95.89% 的交叉验证准确率。 此外，我们与 16 名首次使用 IndexPen 的参与者一起探索了我们的系统对真实世界文本输入的可学习性和适应性，共计 5 次。 每次会议结束后，之前的五用户研究中的预训练模型都会根据迄今为止通过迁移学习为新用户收集的数据进行校准。 F-1 分数显示每次校准后会话平均增加 9.14%，在最后一次会话中 16 个用户平均达到 88.3%。 同时，我们表明用户可以使用 IndexPen 以 86.2% 的准确率键入句子，这是通过字符串相似性来衡量的。 这项工作为未来的交互界面奠定了基础和愿景，可以通过这种范式实现。

- **应用场景：** IndexPen可以在物理尺寸有限的设备上进行空中两指文本输入，不需要在手上佩戴仪器。例如，它可以在自动取款机等公共设备上提供非接触式打字界面，以改善卫生状况。它为在小屏幕上打字提供了一种替代方案，在小屏幕上打字具有挑战性，语音输入不合适或不可行。IndexPen可以识别类似手写的手势，包括30个类。该系统处理微型雷达设备生成的速度和角度轮廓，并使用神经网络检测手势。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_5_fig1.png" alt="image" width ="80%">
    </div>

    - 30种手势的定义：
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_5_fig2.png" alt="image" width ="80%">
    </div>


- **贡献：**
    - <b>1. </b> 介绍了 IndexPen 的设计和功能，它使用户能够通过用食指在拇指面上书写英文字母来输入文本。 它旨在重现用有形工具书写的感觉。 为了获得可接受的打字体验并消除静态噪音，手势集包括 30 个不同的符号（26 个字母和其他实用字符，包括空格、退格键、回车键和激活键）。 激活手势旨在激活和停用 IndexPen 并避免意外输入，我们还包括噪声数据以区分手势和静态噪声。
    
    - <b>2. </b> 详细介绍了我们开发的实时处理pipeline，以支持IndexPen交互范例。它利用了毫米波雷达的两个主要特征集。该模型将这些特征作为混合输入，并使用卷积递归神经网络(CRNN)来解析正在执行的手势。神经网络的预测概率用一种消除抖动算法进行处理，得到类似键盘的字符输入。我们还给出了杂波去除算法的实验结果，该算法显著提高了模型的鲁棒性，并表明IndexPen方法能够区分30个IndexPen符号，在31,000个手势样本中具有高达95.89%的10倍交叉验证精度。

    - <b>3. </b> 调查了实际使用IndexPen的考虑因素，让新用户写出完整的句子。我们通过一系列基于迁移学习的用户特定校准实验，向新用户演示了IndexPen的泛化性。在“留一”实验中，该模型适应新用户的写作，每类20个样本，在5个用户中准确率达到87.55%。我们进一步研究了设计手势的学习性和IndexPen管道在真实文本输入场景中的鲁棒性，16名参与者在不同的日子里进行了5次会议，并通过实验过程收集了他们对IndexPen的建议和反馈。我们通过客观的定量结果和主观的参与者反馈来分析这两个因素，为手势运动检测领域的其他研究者提供了有价值的分析结果。所有参与者的平均F-1分数和最后一个会话的平均字符串相似度分别为0.8815和0.8619。我们的工作解决了在手势运动检测中个体之间未定义的差异。

    
- **整体方案：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_5_fig3.png" alt="image" width ="100%">
    </div>
    - <b>1. 硬件配置</b>  Texas Instrument’s IWR6843AoP，配置Range_res=4.4cm, Velocity_res=0.16m/s

    - <b>2. 杂波去除算法</b> 

    - <b>3. IndexPen神经网络</b> 通过上面解释的传感器信号处理管道，雷达探测到的物体的物理信息以距离-多普勒和距离-方位角-高程剖面表示。当数据流进入时，两个配置文件的序列形成一个动态配置文件，该配置文件以所执行的手势为特征。

    - <b>4. 实时手势检测</b> 输出层的sigmoid激活函数产生一个向量，它表示在过去的120个时间步(即4秒)中，每个手势被写入的概率。



## 4. [mmBP: Contact-free Millimetre-wave Radar based Approach to Blood Pressure Measurement](https://dl.acm.org/doi/10.1145/3560905.3568506)
- **阅读时间：** 2023-3-12

- **出处：** SenSys'22

- **关键词：** 血压，非接触式传感，毫米波

- **Abstract:** Blood pressure (BP) measurement is an indispensable tool in diagnosing and treating many diseases such as cardiovascular failure and stroke. Traditional direct measurement can be invasive, and wearable-based methods may have limitations of discomfort and inconvenience. Contact-free BP measurement has been recently advocated as a promising alternative. In particular, Millimetre-wave (mmWave) sensing has demonstrated its promising potential, however it is confronted with several challenges including noise and vulnerability to human's tiny motions which may occur intentionally and inevitably. In this paper, we propose mmBP, a contact-free mmWave-based BP measurement system with high accuracy and motion robustness. Due to the high frequency and short wavelength, mmWave signals received in the time domain are dramatically susceptible to ambient noise, and deteriorating signal quality. To reduce noise, we propose a novel delay-Doppler domain feature transformation method to exploit mmWave signal's characteristics and features in the delay-Doppler domain to significantly improve signal quality for pulse waveform construction. We also propose a temporal referential functional link adaptive filter leveraging on the periodic and correlation characteristics of pulse waveform signals to alleviate the impact of human's tiny motions. Extensive experiment results achieved by the leave-one-out cross-validation (LOOCV) method demonstrate that mmBP achieves the mean errors of 0.87mmHg and 1.55mmHg for systolic blood pressure (SBP) and diastolic blood pressure (DBP), respectively; and the standard deviation errors of 5.01mmHg and 5.27mmHg for SBP and DBP, respectively.

- **摘要：** 血压 (BP) 测量是诊断和治疗心血管衰竭和中风等多种疾病不可或缺的工具。 传统的直接测量可能是侵入性的，而基于可穿戴设备的方法可能存在不适和不便的局限性。 最近提倡非接触式血压测量作为一种有前途的替代方法。 特别是，毫米波 (mmWave) 传感已展示出其广阔的潜力，但它也面临着一些挑战，包括噪声和易受人类有意且不可避免地发生的微小运动的影响。 在本文中，我们提出了 mmBP，一种基于毫米波的非接触式 BP 测量系统，具有高精度和运动鲁棒性。 由于频率高、波长短，在时域中接收到的毫米波信号极易受到环境噪声的影响，从而降低信号质量。 为了降低噪声，我们提出了一种新颖的延迟多普勒域特征变换方法，以利用毫米波信号在延迟多普勒域中的特性和特征来显着提高脉冲波形构造的信号质量。 我们还提出了一种时间参考功能链接自适应滤波器，利用脉冲波形信号的周期性和相关性特征来减轻人体微小运动的影响。 通过留一法交叉验证 (LOOCV) 方法获得的大量实验结果表明，mmBP 的收缩压 (SBP) 和舒张压 (DBP) 的平均误差分别为 0.87mmHg 和 1.55mmHg； SBP 和 DBP 的标准偏差误差分别为 5.01mmHg 和 5.27mmHg。

- **应用场景：** </br>
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_4_fig1.png" alt="image" width ="90%">
    </div>
    
- **挑战：**
    - <b>1. 从时域中的原始毫米波信号重建高质量脉冲波形具有挑战性。</b>
        - **延迟多普勒(Delay-Doppler, DD)域降噪：** 来自环境的干扰和背景噪音，信号特征可能会失真，使得提取有效的脉冲相关特征变得困难，因此，降噪是毫米波BP测量的关键问题。
    - <b>2. 由于毫米波信号的高工作频率，传统的基于毫米波的方法容易受到身体运动的影响。</b> 小范围或微小的运动(如特发性震颤和静息性震颤)经常在无意中发生带来的干扰。值得注意的是，即使这些震动只导致毫米波雷达与受试者之间的距离变化很小，但它们对无接触毫米波BP测量的性能产生了相当大的影响。
        - **(Nonlinear adaptive filter, NLAF)信号分解算法**，NLAF需要实际的脉冲波形作为参考信号，可能无法直接应用于基于毫米波的 BP 测量，为了解决这个问题，我们提出了一种新方法来生成有效的参考信号，并利用 NLAF 的特性进行 BP 测量。 基本思想是脉冲形态是一种在一段时间内具有高度相关性的周期性重复。 尽管每次重复可能随时间略有不同，但总体模式是稳定的。 但是，当发生微小运动时，趋势和相关性可能不再成立。 这使我们有机会生成与干净的脉冲波形高度相关但与微小运动引起的干扰无关的参考信号。 有了这个参考信号，NLAF就可以有效地减少微小运动对脉搏波形信号的影响。

- **方法总结：**
    为了解决上述挑战，在本文中，我们提出了mmBP，一种基于毫米波的无接触系统，用于安全、高精度和运动鲁棒的BP测量。mmBP执行以下三个步骤。
    - <b>1. </b>使用现成的毫米波雷达(例如，德州仪器，TI IWR1843 BOOST)来捕捉由脉冲活动引起的毫米波反射的变化
    - <b>2. </b>我们将从时域接收到的毫米波信号转移到DD域，然后提取具有代表性的DD域脉冲相关信息并基于噪声和脉冲信号在DD域具有不同属性的事实滤除噪声。
    - <b>3. </b>提出了一种新颖的运动补偿方案，以利用 NLAF 的特性解决微小运动对 BP 测量的影响。 如前所述，由于缺乏参考信号，NLAF 不能直接应用于基于毫米波的 BP 测量。 为了解决这个问题，我们提出了一种新方法来为 NLAF 生成有效的参考信号，然后应用补偿来减少微小运动的影响。


- **贡献：**
    - <b>1. </b> 提出了一种利用毫米波信号特性和 DD 域中的代表性特征的新型 BP 测量系统。 mmBP 完全无接触，不需要佩戴任何设备。 mmBP 能够实现高精度并对微小运动具有鲁棒性，因此有望用于潜在的实际部署。

    - <b>2. </b> 与现有测量方法中常用的时域或频域相比，我们提出了一种新颖的延迟多普勒域特征变换 (DDFT)，以从 DD 域中提取代表性特征以构建脉冲波形。 据我们所知，这是第一个利用 DD 域特征来估计 BP 值的方法。 DDFT能够提高脉冲波形的质量，降低噪声的影响。

    - <b>3. </b>提出了一种时间参考功能链接自适应滤波器（TR-FLAF），以减轻微小运动对脉冲波形构造的影响。 为了获得可靠的滤波性能，我们提出了时间参考信号提取 (TRSE) 算法，通过利用脉冲信号的周期性和相关性来生成非线性自适应滤波器的参考信号。 然后我们应用补偿来减少运动对脉搏信息提取的影响，从而提高 BP 测量的性能。

    - <b>4. </b>进行了广泛的实验来评估 mmBP 在各种场景和设置下的性能。 结果表明mmBP对于SBP和DBP的平均误差分别为0.87mmHg和1.55mmHg； SBP 和 DBP 的标准偏差误差分别为 5.01mmHg 和 5.27mmHg。
    
- **整体方案：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_4_fig2.png" alt="image" width ="90%">
    </div>

    - <b>1. mmWave Reflection Capturing</b> 根据接收到的毫米波反射捕获动脉脉冲信号。毫米波信号由于频率高、带宽大，可以有效地反映脉冲运动引起的皮肤位移，这对于脉冲波形的构建至关重要。由于脉冲信号（例如，波形）包含足够的 BP 相关信息，因此可以对其进行处理以测量 BP 值并跟踪其变化。
    

    - <b>2. DD Domain Feature Transformation (DDFT)</b>将前一步得到的脉冲信号从时域转换到DD域，实现降噪。由于期望脉冲信号与噪声具有不同的时延和多普勒响应，因此可以在DD域中保留期望信号并减少噪声的影响，从而增强脉冲波形的构造。
        - (a) Wigner变换操作将𝜙(𝑡)从时域映射到时频(TF)域。参考论文公式5.
        - (b) STFT，参考论文公式6.
    

    - <b>3. Motion Compensation</b>这一步消除了微小运动对脉冲波形构造的影响。为此，我们提出了一种时域参考功能链自适应滤波器(TR-FLAF)来缓解由微小运动引起的非线性影响。特别地，我们提出了一种时域参考功能链自适应滤波器(TR-FLAF)，滤除微小运动引起的非线性影响，增强所需信号，构建精确的脉冲波形。
    -   <div style="text-align:center">
            <img src="/assets/paperNotes_images/D2023_4_fig3.png" alt="image" width ="90%">
        </div>

        - Temporal Reference Signal Extraction.
        - Functional Expansion Block.
        - Coefficient Adaptation.

    - <b>4. BP Estimation (回归预测)</b>最后一步首先从脉冲波形中提取6个可区分的DD特征，这些特征代表了BP活动的独特属性。然后，我们将这些特征输入一个回归模型，找到提取的特征与BP值之间的有效关系，实现了成功的BP测量。六个特征为：
        - (1) 最大峰值(MP): MP是脉冲波形在DD域的最高点，对应于收缩压(Systolic Blood Pressure, SBP)。
        - (2) 第一拐点(FIP): FIP是脉冲信号在DD域中的第一个拐点，它与舒张压(Diastolic Blood Pressure, DBP)有关。
        - (3) 最大最小比 (MMR)：MMR 测量为 DD 域中脉冲波形的最大信号值与最小信号值的比值，它反映了该脉冲周期强度的变化。
        - (4) 最大值与拐点比 (MIR)：MIR 定义为 DD 域中脉冲波形的最大值与第一拐点信号值之比，对应于动脉上的波反射。
        - (5) 峰峰值间隔（PPI）：PPI是DD域中脉搏波形峰峰值间隔的量度，可以用来表示一个完整的脉搏波形。
        - (6) 期望和方差：期望是DD域中脉冲波形的平均值，方差是期望周围的变异量。 两者都反映了脉搏信号的统计特征。

    - 综上所述，可以看出，这六个特征可以全面反映脉冲波形的关键特征，这对于实现可靠的BP估计至关重要。请注意，选择额外的特征可能会导致BP测量的改进，但它会带来更多的过程复杂性。


- **读后感：** 
    - 特征提取算法DD域：Wigner+STFT
    - 动态干扰去除：TR-FLAF算法

- **Cite：** 
```
@inproceedings{10.1145/3560905.3568506,
author = {Shi, Zhenguo and Gu, Tao and Zhang, Yu and Zhang, Xi},
title = {MmBP: Contact-Free Millimetre-Wave Radar Based Approach to Blood Pressure Measurement},
year = {2023},
isbn = {9781450398862},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3560905.3568506},
doi = {10.1145/3560905.3568506},
abstract = {Blood pressure (BP) measurement is an indispensable tool in diagnosing and treating many diseases such as cardiovascular failure and stroke. Traditional direct measurement can be invasive, and wearable-based methods may have limitations of discomfort and inconvenience. Contact-free BP measurement has been recently advocated as a promising alternative. In particular, Millimetre-wave (mmWave) sensing has demonstrated its promising potential, however it is confronted with several challenges including noise and vulnerability to human's tiny motions which may occur intentionally and inevitably. In this paper, we propose mmBP, a contact-free mmWave-based BP measurement system with high accuracy and motion robustness. Due to the high frequency and short wavelength, mmWave signals received in the time domain are dramatically susceptible to ambient noise, and deteriorating signal quality. To reduce noise, we propose a novel delay-Doppler domain feature transformation method to exploit mmWave signal's characteristics and features in the delay-Doppler domain to significantly improve signal quality for pulse waveform construction. We also propose a temporal referential functional link adaptive filter leveraging on the periodic and correlation characteristics of pulse waveform signals to alleviate the impact of human's tiny motions. Extensive experiment results achieved by the leave-one-out cross-validation (LOOCV) method demonstrate that mmBP achieves the mean errors of 0.87mmHg and 1.55mmHg for systolic blood pressure (SBP) and diastolic blood pressure (DBP), respectively; and the standard deviation errors of 5.01mmHg and 5.27mmHg for SBP and DBP, respectively.},
booktitle = {Proceedings of the 20th ACM Conference on Embedded Networked Sensor Systems},
pages = {667–681},
numpages = {15},
keywords = {contact-free sensing, mmWave, blood pressure},
location = {Boston, Massachusetts},
series = {SenSys '22}
}
```


## 3. [OmniScatter: Extreme Sensitivity mmWave Backscattering Using Commodity FMCW Radar](https://dl.acm.org/doi/10.1145/3498361.3538924)
- **[Youtbe]()**

- **阅读时间：** 2022-3-5

- **出处：** MobiSys’22, June 25–July 1

- **关键词：** mmWave，毫米波背向散射

- **摘要：** 大规模连接是物联网成功的关键。 虽然毫米波反向散射具有巨大的潜力，但大量的信号衰减和压倒性的环境反射带来了重大挑战。 我们展示了 OmniScatter，这是一种实用的毫米波反向散射，具有 -115 dBm 的极高灵敏度。 该性能在理论上可与流行的商品 RFID EPC Gen2 (900 MHz) 相媲美，并通过在具有大量环境反射和阻塞的各种实际设置下的评估进行了经验验证 - 例如，在办公室中，标签被锁在 6 米外的木制壁橱中 ，以及在图书馆和零售店中，标签被放置在两排金属架子上。 OmniScatter 的核心是新的高清 FMCW (HD-FMCW)，它与标签 (FSK) 信号相互作用，以在频域中消除来自标签信号的环境反射，从本质上提供对环境反射的免疫力。 为了进一步支持实际部署，OmniScatter 提供无需协调的频分多址 (FDMA)，可轻松扩展至数千个并发标签。 阅读器建立在商品雷达上，而标签原型则建立在 PCB 上。 跟踪驱动的评估展示了 1100 个标签的并发通信，BER < 1.5%，为日常和任何地方使用的实用毫米波反向散射铺平了道路。

- **应用场景：** </br>
    <!-- <div style="text-align:center">
        <img src="/assets/paperNotes_images/ _fig1.png" alt="image" width ="100%">
    </div> -->
    
- **动机：** FMCW通过利用跨越整个带宽的Chirp，提供了大量的编码增益，以潜在地帮助低功率后向散射信号，否则无法检测到。然而，典型的室内空间，如家庭、办公室、商场和医院，有一个复杂的环境，有丰富的环境反射，它们很快就会累积成大量的杂波噪声。这本质上造成了强的自干扰，很容易压倒弱的后向散射信号。

- **挑战：**
    - <b>1. 信号高传输损失</b>
    - <b>2. </b>
    - <b>3. </b>
    - <b>4. </b>

- **贡献：**
    - <b>1. </b> 设计了OmniScatter，它独特地结合了极高的灵敏度和无需协调的部署，用于野外的实际毫米波后向散射。
    - <b>2. </b> OmniScatter的新型HD-FMCW雷达有效地将FSK标签信号从杂波噪声中分离出来，灵敏度达到-115 dBm。这是实现稳健毫米波反向散射通信和以被动方式有效利用毫米波带宽的基础技术。
    - <b>3. </b> 使用商用mmwave雷达，阅读器标签在PCB (24 GHz)和商用射频开关(60 GHz)上进行了原型制作。在各种真实环境中进行了广泛的测试床评估，并进行了具有1100个并发标记的跟踪驱动的大规模模拟。
    - <b>4. </b>
    
- **整体方案：**
    主要包含两部分内容：High Definition FMCW  和  Coordination-free FDMA
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_3_fig2.png" alt="image" width ="90%">
    </div>

    - <b>1. High Definition FMCW (HD-FMCW)</b> HD-FMCW 与原始 FMCW 的主要区别在于两个方面：
        - (i) 无chirp间隔：HD-FMCW 每个符号包含一系列线性调频信号，没有线性调频间隔，这与 FMCW 中具有保护时间的单线性调频符号相反。 
        - (ii) 符号内相位连续性：相位在符号内的整个chirp中保持连续。 即，线性调频信号开始和结束的相位在 HD-FMCW 中匹配，以实现线性调频信号之间的周期性。    
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_3_fig1.png" alt="image" width ="90%">
    </div>
     
    - <b>2. Coordination-free FDMA（无协调FDMA）</b>


- **思维导图：**
    <!-- <div style="text-align:center">
        <img src="/assets/paperNotes_images/ _fig3.png" alt="image" width ="100%">
    </div> -->

- **读后感：** 



## 2. [AmbiEar: mmWave Based Voice Recognition in NLoS Scenarios](https://dl.acm.org/doi/abs/10.1145/3550320)

- **阅读时间：** 2023-2-25

- **出处：** UbiComp'22

- **关键词：** 毫米波进行非视距（NLos）的语音识别

- **摘要：** 基于毫米波 (mmWave) 的传感是一项重要技术，可实现创新的智能应用，例如语音识别。 该领域的现有工作需要直接感测人类的近喉区域，因此在非视线 (NLoS) 场景中的适用性有限。 本文提出了 AmbiEar，这是第一个适用于 NLoS 场景的基于毫米波的语音识别方法。 AmbiEar 基于这样一种认识，即无论人的位置和姿势如何，人的声音都会引起周围物体的相关振动。 因此，AmbiEar将周围的物体视为可以感知声音的耳朵，通过感知周围物体的振动，实现对人声的间接感知。 通过结合公共组件提取、信号叠加和编码器-解码器网络等设计，AmbiEar 解决了低信噪比和失真信号带来的挑战。 我们在商用毫米波雷达上实施 AmbiEar，并评估其在不同设置下的性能。 实验结果表明，与直接感知方法相比，AmbiEar 在 NLoS 场景中的词识别准确率为 87.21%，识别错误减少了 35.1%。

- **应用场景：** </br> 为了使基于毫米波的语音识别真正适用于实践，下图描绘了一个典型的场景。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_2_fig1.png" alt="image" width ="100%">
    </div>
    
- **动机：** 我们观察到一个有趣的现象:声音以机械波的形式传播。人的声音会引起周围物体的振动，其中包含与人的声音高度相关的常见成分。受此启发，我们提出了AmbiEar，一种基于毫米波的语音识别间接传感方法。AmbiEar将周围的物体转换为周围的“耳朵”，并使用毫米波雷达感知“耳朵”发出的与语音相关的信号，从而实现语音识别。AmbiEar专为但不限于NLoS场景而设计。由于AmbiEar利用周围物体进行语音识别，因此它在LoS场景下也能很好地工作。

- **挑战：**
    - <b>1. </b> AmbiEar 根据反射信号中不同的动态来区分人和周围物体
    - <b>2. </b> AmbiEar提取并组合来自多个物体的振动信号的公共成分

- **贡献：**
    - <b>1. </b> 我们提出了毫米波间接感知的概念，将周围物体转换为“耳朵”，帮助我们感知。据我们所知，AmbiEar是首个在NLoS场景下基于毫米波的语音识别方法。
    - <b>2. </b> AmbiEar的设计有效地解决了一系列技术难题。我们特别关注了如何利用低信噪比和语义不完整的振动信号进行语音识别的问题。AmbiEar的定制化设计主要包括四个部分:环境检测、公共分量提取、信号叠加和语音识别。
    - <b>3. </b> 我们在商业设备（TI IWR1642 板）上实现了 AmbiEar，并在各种设置下进行了大量实验。 结果表明，AmbiEar 实现了 87.21% 的单词识别准确率和 88.66% 的字符识别准确率。 AmbiEar 显着提高了基于毫米波的语音识别在实践中的适用性。
    
- **整体方案：**
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_2_fig2.png" alt="image" width ="100%">
    </div>
    - <b>1. Surroundings Detection</b> AmbiEar 首先扫描环境以获得所有物体的信息，包括它们的位置和反射信号强度。 然后它不断跟踪物体的位置，并根据轨迹的变化选择人的位置。 之后，AmbiEar 可以选择特定范围内的周围物体作为下一步的反射体。在跟踪人的位置后，AmbiEar会尝试在人的位置周围的特定范围(例如1m)内找到静态物体。
    
    - <b>2. Common Component Extraction==》MVDR算法</b> AmbiEar首先从这些选定的反射器中提取反射信号。然后提取这些信号的公共分量以抵抗低信噪比。AmbiEar应用接收波束形成算法从这些静态物体中提取反射信号。
    
    - <b>3. Signal Superimposition ==》圆拟合算法</b> 为了进一步抵御环境声噪声的影响，AmbiEar将环境声噪声与环境声噪声进行叠加，得到叠加时频谱图。为了进一步抵抗低信噪比，AmbiEar对这些IQ采样点执行圆拟合算法。
   
    - <b>4. Voice Recognition</b> 通过上述步骤，AmbiEar获得了用户声音引起的增强振动信号的时频谱图。应考虑振动信号和语义信息的错位。
        <div style="text-align:center">
            <img src="/assets/paperNotes_images/D2023_2_fig3.png" alt="image" width ="100%">
        </div>


## 1. [Adaptive and Fast Combined Waveform-Beamforming Design for MMWave Automotive Joint Communication-Radar](https://ieeexplore.ieee.org/document/9398548)

- **阅读时间：** 2023-2-19

- **出处：** IEEE Journal of Selected Topics in Signal Processing （中科院2区）

- **关键词：** 压缩感知，自动驾驶中的毫米波mmWave

- **摘要：** 毫米波 (mmWave) 联合通信雷达 (JCR) 将为自动驾驶等应用实现高数据速率通信和高分辨率雷达传感。 然而，基于毫米波通信硬件的现有 JCR 系统由于采用了定向通信波束，因此存在角视场有限和雷达估计精度低的问题。 在本文中，我们提出了一种适用于毫米波汽车 JCR 的自适应和快速组合波形波束形成设计，其相控阵架构允许在通信和雷达性能之间进行权衡。 为了快速估计具有宽视场的多普勒角域中的毫米波汽车雷达通道，我们的 JCR 设计采用发射波束形成器的循环偏移来获取雷达通道测量值，并在 时空维度。 在我们问题的时空采样约束下，我们优化这些循环偏移以最小化 CS 矩阵的相干性。 我们使用用于雷达估计的归一化均方误差 (MSE) 度量和用于数据通信的失真 MSE 度量来评估 JCR 性能权衡，这类似于率失真理论中的失真度量。 此外，我们为自适应 JCR 组合波形波束形成设计开发了基于 MSE 的加权平均优化问题。 数值结果表明，我们提出的 JCR 设计能够以低归一化 MSE 估计多普勒角域中的短程和中程雷达信道，但代价是通信失真 MSE 的小幅下降。

- **应用场景：** </br> 汽车毫米波 JCR 系统的图示，该系统同时执行具有宽 FoV 的 SRR/MRR 雷达感测和具有窄 FoV 的 V2V 通信。我们考虑这样的用例：源车辆发送毫米波 JCR 波形与距离 D 处以相对速度 V 移动的接收车辆通信，同时使用接收到的回波进行汽车雷达传感。
    <div style="text-align:center">
        <img src="/assets/paperNotes_images/D2023_1_fig1.jpg" alt="image" width ="100%">
    </div>
    
- **动机：** 在自动驾驶中毫米波通信和感知的协同工作问题，在最小毫米波通信性能的约束下，优化毫米波的感知性能。

- **贡献：**
    - <b>1. 系统架构</b> 作者为毫米波自动驾驶JCR系统提出了一种新的架构，该系统在不会太大降低通信数据速率同时，可在宽FoV中执行汽车MRR和SRR感知。 该架构捕获了多普勒角域中具有多个目标的稀疏毫米波 JCR 信道的细微差别。 我们提出的 JCR 系统采用通用 TX 波形结构，并使用可调谐 TX 波束成形设计，可以优化以使用稀疏传感技术实现增强的 JCR 性能。
    
    - <b>2. 卷积压缩感知方法</b> 作者开发了一种卷积 CS (CCS)-JCR 技术来估计多普勒角域中的二维雷达通道。 在这种技术中，发射器应用 JCR TX 波束形成器的循环偏移以在雷达接收器处获取 CS 测量值。 将 CS 问题转换为 2D 中的部分傅立叶 CS 问题。问题中的时空传感约束只允许比具有可比尺寸的一般 2D 部分傅立叶 CS 问题更少的子采样位置配置。
    
    - <b>3. 优化的卷积压缩感知</b> 提出了一种优化的CCS (OCCS)-JCR方法，通过仔细设计在发射机上应用的循环位移来实现优越的多普勒角域信道重建。在我们所开发的JCR系统模型的时空感知约束下，优化的循环位移导致部分傅里叶CS的时空采样模式达到最小相干性。

    - <b>4. 性能度量方法</b> 使用雷达的归一化MSE (NMSE)度量和通信的可比失真MSE (DMSE)度量来研究JCR性能权衡，使用分析和模拟。此外，我们为满足帕累托最优界限的汽车应用中的自适应组合波形波束形成毫米波 JCR 设计制定了基于 MSE 的加权平均优化问题。我们针对不同目标场景中提出的 OCCS-JCR 方法解决了基于 MSE 的优化问题。

    - <b>5. 实验结果 </b> 数值结果表明，所提出的 OCCS-JCR 组合波形和波束形成设计以低 NMSE 的多普勒角域估计 MRR 和 SRR 雷达信道，代价是通信 DMSE 略有减少。 所提出的 OCCS-JCR 性能最好，其次是使用随机循环偏移的随机 CCS (RCCS)-JCR，扩展用于多普勒角域雷达信道估计的 RSJCR 性能最差。
    
- **整体方案：**
    - <b>1. 系统模型</b>
        - A. 波形设计(前导码+数据)
        - B. JCR的波束形成器设计
        - C. 接收信号模型：通信接收信号模型 + 雷达接收信号模型

    - <b>2. </b> 在雷达配置中的卷积压缩感知（CCS），由于毫米波频率下环境的传播特性，当用适当的基表示时，信道近似稀疏。



