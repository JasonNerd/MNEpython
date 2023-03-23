# 2023-03-17更新
今年2月以来，重心偏向脑信号的处理技术与软件系统的研究，同时还陆陆续续的看了些Java的编程基础。总choPY体来说，浑浑噩噩中找到了些许方向，了解了例如PsychoPy的心理学实验范式设计与实时刺激呈现平台，例如OPenViBE的脑电信号数据采集、传输和存储程序, 较为详细地学习了例如EEGLab这样的基于MatLab的脑电数据预处理程序包 -- 它包含丰富的信号处理方法与可视化程序, 提供的信号处理功能主要是滤波、坏导去除、信号重参考、独立成分分析去除伪迹，当然还包含例如ERP分析的内容。

那么 EEGLab 仅仅提供的是一些头皮脑电信号地处理, 主要是信号去噪, 同时包含一些心理学实验的范式设计。还不涉及特征分析提取与分类，很难想象要如何从这样芜杂的波形图去解释一些信息。

因此，在借助EEGLab的学习对脑信号分析有一定的了解后，我想立即中断，并转而去学习更新更现代化的 **`MNE-Python`**。同时, 对于Java和算法的学习, 再一次再一次的捡起来（不知道中间断了几次了）

## 03-20的新指示
1. 调研MNE和EEGLAB的功能, 一整个的数据处理流程, 尤其是能够做哪些可视化, 哪些能够直接集成, 二者之间的 --- pipe_line
2. 明确基本任务要求是要开发一个可重用的有界面交互的开发框架, 先得有一个架子, 一方面可以是基于 MATLAB 的工具库, 另一方面也可以是基于 Python 的工具库, 此外还可以是独立的程序软件
3. 明确根本任务要求是开发一个用户友好的、多数据兼容的、基于侵入式BCI数据处理的程序软件。

关于第1条, 目前看来需要做以下工作:
1. 理清楚常见的几种心理学实验范式, 除了基本的实验设计和功能性特点，还要对他们的数据存储模式进行调研，存了哪些内容，不同的范式怎么统一的
2. 其次，可以直接对现有的常见的数据格式进行调研，注意 marker 等一些内容怎么存储的

### 关于MNE
Open-source Python package for exploring, visualizing, and analyzing human neurophysiological data: MEG, EEG, sEEG, ECoG, NIRS, and more.

