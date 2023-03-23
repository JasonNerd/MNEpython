# 2023-03-17更新
今年2月以来，重心偏向脑信号的处理技术与软件系统的研究，同时还陆陆续续的看了些Java的编程基础。总choPY体来说，浑浑噩噩中找到了些许方向，了解了例如PsychoPy的心理学实验范式设计与实时刺激呈现平台，例如OPenViBE的脑电信号数据采集、传输和存储程序, 较为详细地学习了例如EEGLab这样的基于MatLab的脑电数据预处理程序包 -- 它包含丰富的信号处理方法与可视化程序, 提供的信号处理功能主要是滤波、坏导去除、信号重参考、独立成分分析去除伪迹，当然还包含例如ERP分析的内容。

那么 EEGLab 仅仅提供的是一些头皮脑电信号地处理, 主要是信号去噪, 同时包含一些心理学实验的范式设计。还不涉及特征分析提取与分类，很难想象要如何从这样芜杂的波形图去解释一些信息。

因此，在借助EEGLab的学习对脑信号分析有一定的了解后，我想立即中断，并转而去学习更新更现代化的 **`MNE-Python`**。同时, 对于Java和算法的学习, 再一次再一次的捡起来（不知道中间断了几次了）