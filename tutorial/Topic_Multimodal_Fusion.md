# 多模态融合（MultiModal Fusion）

---
## 1. 多模态学习

### 目标：多模态融合技术的主要目标是缩小语义子空间中的分布差距，同时保持模态特定语义的完整性。


为了使人工智能进一步加强对我们周边事物的理解，它需要具备解释多模态信号的能力。一般多模态需要处理的任务主要如上图有：

- 表征（Representation） 找到某种对多模态信息的统一表示，分Coordinated representations（每个模态各自映射然后用相关度距离来约束表示），Joint representations（多个模态一起映射）。

- 翻译（Translation） 一个模态映射到另一个模态，分example-based（有候选集，如检索任务），generative（Decoder-Encoder）。

- 对齐（Alignment） 找模态子成份之间的关系，如某词对应某区域。分显式对齐和隐式对齐，Attention首当其冲。

- 融合（Fusion） 整合信息，分model-agnostic（早晚融合），model-based（融合更深入），也是本篇要整理的内容。

- 联合学习（Co-learning）。通过利用丰富的模态的知识来辅助稀缺的模态，分parallel（如迁移学习），non-parallel（迁移学习，zero shot），hybrid。

一般来说，模态是指事物发生或存在的方式，多模态是指两个或者两个以上的模态的各种形式的组合。对每一种信息的来源或者形式，都可以称为一种模态（Modality），目前研究领域中主要是对图像，文本，语音三种模态的处理。之所以要对模态进行融合，是因为不同模态的表现方式不一样，看待事物的角度也会不一样，所以存在一些交叉（所以存在信息冗余），互补（所以比单特征更优秀）的现象，甚至模态间可能还存在多种不同的信息交互，如果能合理的处理多模态信息，就能得到丰富特征信息。即概括来说多模态的显著特点是： 冗余性 和 互补性 。

---
## 2. 多模态融合架构（神经网络模型的基本结构形式）

多模态融合的主要目标是缩小模态间的异质性差异，同时保持各模态特定语义的完整性，并在深度学习模型中取得最优的性能。多模态融合架构分为三类：联合架构、协作架构和编解码架构。


### 联合架构（Joint Architecture）
多模态融合的策略是集成不同类型的特征来提高机器学习模型性能， 弥补不同模态的异质性差异。联合架构是将多模态空间映射到共享语义子空间中，从而融合多个模态特征

- 加联合：多模态联合架构的关键是实现特征“联合”，最简单方法是直接连接，即“加”联合方法。该方法在不同的隐藏层实现共享语义子空间，将转换后的各个单模态特征向量语义组合在一起，从而实现多模态融合 $$z = f(w^T_1v_1+...+w^T_nv_n)$$ 其中$z$是共享语义子空间中的输出结果,$v$是各单模态的输入，$w$是权重，下标表示不同的模态，通过映射$f$将所有子模态语义转换到共享子空间。

- 乘联合：$$z=\begin{bmatrix} v^1 \\ \vdots  \\ 1 \end{bmatrix} \otimes  \cdots \otimes \begin{bmatrix} v^1 \\ \vdots  \\ 1  \end{bmatrix}$$ 尽管“加”联合方法简单且容易实现，但其特征向量语义组合易造成后期语义丢失，使模型性能降低。而“乘”联合方法弥补了这一不足，通过张量计算使特征语义得到更“充分”融合，最常见的方法是深度神经网络 

多模态联合框架的优点是融合方式简单，且共享子空间往往具备语义不变性，有助于在机器学习模型中将知识从一种模态转移到另一种模态。缺点是各单模态语义完整性不易在早期发现和处理。


### 协同架构（Coordinated Architecture）
协同架构包括跨模态相似模型和典型相关分析，其目的是寻求协调子空间中模态间的关联关系；由于不同模态包含的信息不一样，协同方法有利于保持各单模态独有的特征和排它性。协同架构在跨模态学习中已经得到广泛应用，主流的协同方法是基于交叉模态相似性方法，该方法旨在通过直接测量向量与不同模态的距离来学习一个公共子空间[32]。而基于交叉模态相关性的方法旨在学习一个共享子空间，从而使不同模态表示集的相关性最大化[4]。
交叉模态相似性方法在相似性度量的约束下保持模态间和模态内的相似性结构，期望相同语义或相关对象的跨模态相似距离尽可能小，不同语义的距离尽可能大。



### 编解码架构（Encode-Decode Architecture）
编解码器架构是用于将一个模态映射到另一个模态的中间表示。
编码器将源模态映射到向量 v 中，解码器基于向量 v 将生成一个新的目标模态样本。该架构在图像标注、图像合成、视频解码等领域有广泛应用。

目前，编解码器架构在研究中重点关注共享语义捕获和多模序列的编解码两个问题。为了更有效地捕获两种模态的共享语义，一种流行的解决方案是通过一些正则化术语保持模态之间的语义一致性。必须确保编码器能正确地检测和编码信息，而解码器将负责推理高级语义和生成语法，以保证源模态中语义的正确理解和目标模态中新样本的生成。为了解决多模序列的编码和解码问题，关键是训练一个灵活的特征选择模块，而训练序列的编码或解码可以看作一个顺序决策问题，因此通常会采用决策能力强的模型和方法解决。例如，深度强化学习(Deep Reinforcement Learning，DRL)是一种常用的多模序列编解工具。

与其它框架相比，编解码器框架的优点是能够在源模态基础上生成新的目标模态样本。其缺点是每个编码器和解码器只能编码其中一种模态。 此外，决策模块设计非常复杂，值得研究者进一步关注。


## 3. 多模态融合方法
### 早期融合
早期融合在提取特征后立即集成特征（通常只需连接各模态特征的表示）即特征融合。由于深度学习本质上会涉及从原始数据中学习特征的具体表示，这就导致了有时可能在没有抽取特征之前就需要进行融合，即数据融合。因此，特征层面和数据层面的融合都称为早期融合。模态之间往往是高度相关的，但这种相关性在特征层和数据层提取难度都很大。

### 晚期融合
晚期融合在每种模式输出结果（例如输出分类或回归结果）之后才执行集成。晚期融合也叫决策级融合，深度学习模型先对不同的模态进行训练，再融合多个模型输出的结果。因为该方法的融合过程与特征无关，且来自多个模型的错误通常是不相关的，因此这种融合方法往往受到青睐。

### 混合融合
混合融合结合了早期融合方法和单模态预测器的输出。
混合融合结合了早期和晚期融合方法，在综合了二者优点的同时，也增加了模型的结构复杂度和训练难度。由于深度学习模型结构的多样性和灵活性，比较适合使用混合融合方法，在多媒体、图像问答任务、手势识别等领域应用得非常广泛。


---
## 相关论文

1. TFN (Multimodal Tensor Fusion Network)
是基于矩阵的TFN，TFN属于early fusion，是一个典型通过矩阵运算进行融合特征融合的多模态网络，即直接对三种模态的数据（如Text，Image，Audio）的三个特征向量X，Y，Z，进行：$$z=\begin{bmatrix} h^x \\  1 \end{bmatrix}  \otimes \begin{bmatrix} h^y \\   1  \end{bmatrix} \otimes \begin{bmatrix} h^z \\ 1 \end{bmatrix}  $$ 融合后的结果为：
    <div style="text-align:center">
        <p align="center">
            <img src="imgs/Topic_Multimodal_Fusion/ multimodal_joint_fig1.png", width="80%">
        </p>
    </div>
    缺点：TFN通过模态之间的张量外积（Outer product）计算不同模态的元素之间的相关性，但会极大的增加特征向量的维度，造成模型过大，难以训练。



2. [Low Rank Fusion based Transformers for Multimodal Sequences](https://aclanthology.org/2020.challengehml-1.4.pdf)

    - 摘要：是TFN的等价升级版，就具体模型如图。LMF利用对权重进行低秩矩阵分解，将TFN先张量外积再FC的过程变为每个模态先单独线性变换之后再多维度点积，可以看作是多个低秩向量的结果的和，从而减少了模型中的参数数量。
    <div style="text-align:center">
      <p align="center">
        <img src="imgs/Topic_Multimodal_Fusion/multimodal_joint_fig2.png", width="80%">
       </p>
    </div>


3. [Efficient Low-rank Multimodal Fusion with Modality-Specific Factors](https://arxiv.org/abs/1806.00064)

    - [Low Rank Fusion based Transformers for Multimodal Sequences](https://aclanthology.org/2020.challengehml-1.4.pdf)

4. [MERLOT Reserve: Neural Script Knowledge through Vision and Language and Sound](https://arxiv.org/abs/2201.02639)

    - CVPR2022


5. [An Empirical Study of Training End-to-End Vision-and-Language Transformers](https://arxiv.org/abs/2111.02387)

    - METER (Multimodal End-to-end TransformER framework)
    - CVPR2022

    <div style="text-align:center">
        <p align="center">
            <img src="imgs/Topic_Multimodal_Fusion/vl-FUSION_fig1.png", width="80%">
        </p>
     </div>

    - 摘要：视觉和语言 (VL) 预训练已被证明对各种 VL 下游任务非常有效。虽然最近的工作表明完全基于变压器的 VL 模型比以前基于区域特征的方法更有效，但它们在下游任务上的性能通常会显着下降。在本文中，我们提出了 METER，一个多模式端到端 Transformer 框架，通过它我们研究如何以端到端的方式设计和预训练一个完全基于 Transformer 的 VL 模型。具体来说，我们从多个维度剖析模型设计：视觉编码器（例如，CLIP-ViT、Swin Transformer）、文本编码器（例如，RoBERTa、DeBERTa）、多模态融合模块（例如，合并注意力与共同注意力）、架构设计（例如，仅编码器与编码器-解码器）和预训练目标（例如，蒙版图像建模）。我们进行了全面的实验，并提供了有关如何训练高性能 VL 变压器的见解。 METER 仅使用 4M 图像进行预训练，在 VQAv2 测试标准集上实现了 77.64% 的准确率，超过了最先进的基于区域特征的模型 1.04%，并且优于之前最好的全变压器-基于模型的 1.6%。值得注意的是，当进一步扩大规模时，我们最好的 VQA 模型达到了 80.54% 的准确度。代码和预训练模型在 https://github.com/zdou0830/METER. 上发布。

    - 模型架构
        - Vision Encoder  --> [ViTs](https://arxiv.org/abs/2010.11929)</br>
          [Vision Transformer 超详细解读 (原理分析+代码解读) (一)](https://zhuanlan.zhihu.com/p/340149804)

        - Text Encoder  --> [BERT]() and [RoBERT]()

        - Multimodal Fusion（两种特征融合方法）
        <div style="text-align:center">
        <p align="center">
        <img src="imgs/Topic_Multimodal_Fusion/vl-FUSION_fig2.png", width="80%">
        </p>
        </div>
            

        - Encoder-Only vs. Encoder-Decoder

6. [L-Verse: Bidirectional Generation Between Image and Text](https://arxiv.org/abs/2111.11133) 

    - CVPR2022

7. [NLX-GPT: A Model for Natural Language Explanations in Vision and Vision-Language Tasks](https://arxiv.org/abs/2203.05081)
    - CVPR2022
    ```bibtex
    
    ```


8. [Conditional Prompt Learning for Vision-Language Models](https://arxiv.org/abs/2203.05557)
    - CVPR2022
    ```bibtex

    ```

9. [UNITER: UNiversal Image-TExt Representation Learning](https://arxiv.org/abs/1909.11740)
    - UNITER：通用图像-文本表示学习
    - UNITER (UNiversal Image-TExt Representation)
    - ECCV2020
    - 摘要：联合图像-文本嵌入是大多数视觉和语言 (V+L) 任务的基础，其中同时处理多模态输入以实现联合视觉和文本理解。在本文中，我们介绍了 UNITER，一种通用的图像文本表示，通过对四个图像文本数据集（COCO、视觉基因组、概念字幕和 SBU 字幕）的大规模预训练学习，它可以为异构下游 V+ 提供动力L 个具有联合多模态嵌入的任务。我们设计了四个预训练任务：掩蔽语言建模 (MLM)、掩蔽区域建模 (MRM，具有三个变体)、图像-文本匹配 (ITM) 和词区域对齐 (WRA)。与之前将联合随机掩蔽应用于两种模式的工作不同，我们在预训练任务上使用条件掩蔽（即，掩蔽语言/区域建模以对图像/文本的全面观察为条件）。除了用于全局图像-文本对齐的 ITM 之外，我们还通过使用最优传输 (OT) 提出 WRA，以在预训练期间明确鼓励单词和图像区域之间的细粒度对齐。综合分析表明，条件掩蔽和基于 OT 的 WRA 都有助于更好的预训练。我们还进行了彻底的消融研究，以找到预训练任务的最佳组合。大量实验表明，UNITER 在 6 个 V+L 任务（超过 9 个数据集）上实现了最新的技术水平，包括视觉问答、图像文本检索、引用表达理解、视觉常识推理、视觉蕴含和 NLVR2。此 https URL 上提供了代码。

    <div style="text-align:center">
    <p align="center">
        <img src="imgs/Topic_Multimodal_Fusion/UNITER_fig1.png", width="80%">
    </p>
    </div>


10. [](https://arxiv.org/abs/1704.06567)
    - ACL2017




11. [](https://schlr.cnki.net/Detail/index/SJPD_04/SJPDC30D2BBA5D56D1AB09D357D1A3DEC122)
    - AAAI2019



12. [Attentional Feature Fusion](https://arxiv.org/pdf/2009.14082.pdf)


13. [Multimodal Transformer for Unaligned Multimodal Language Sequences](https://arxiv.org/pdf/1906.00295.pdf)


14. [Beyond Shared Subspace: A View-Specific Fusion for Multi-View Multi-Label Learning](https://www.aaai.org/AAAI22Papers/AAAI-500.LyuG.pdf)
    - AAAI2022


15. [TransMEF: A Transformer-Based Multi-Exposure Image Fusion Framework using Self-Supervised Multi-Task Learning](https://arxiv.org/pdf/2112.01030v2.pdf)



16. [Reference-Based Speech Enhancement via Feature Alignment and Fusion Network](https://www.aaai.org/AAAI22Papers/AAAI-3711.YueH.pdf)














