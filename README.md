## 基于条件生成对抗网络的低照度彩色图像增强算法
本项目提供了我们发表在《红外与激光工程》期刊上的《基于条件生成对抗网络的低照度彩色图像增强算法》代码与数据集。

# 摘要
针对低照度条件下的彩色图像增强问题，提出一种基于条件生成对抗网络的低照度图像增强算法。首先，设计了集成密集连接残差模块和注意力机制模块的生成器网络，更加关注低照度图像中的重要目标特征；然后，构建了基于选择性卷积核的判别器网络，使得判别器能够根据输入自适应地调整其感受野大小；接着，通过设计Prewitt边缘损失项和 YUV 色度损失项分别增强了网络模型对于图像边缘细节的提取能力和对图像色彩畸变的消除能力；最后，在 LOL 公开数据集上对本文算法分别进行了定性和定量测试。实验结果表明：与目前基于深度学习的低照度彩色图像增强算法相比，本文算法在峰值信噪比、结构相似度和色差等指标上分别提升了32.7%、57.5% 和48.45%，能够较好地克服低照度成像条件下的图像噪声与色偏干扰问题。
![绘图1](https://github.com/user-attachments/assets/e9e04cbd-20a1-42d2-9f0d-b21a0c874a5e)

# 结果
我们利用LOL数据集对本文算法进行了测试，测试结果如下图所示：
![11](https://github.com/user-attachments/assets/ec2d1289-84fb-4026-bca2-0832ca115373)

# 运行
（1）下载本项目后，对data文件夹中的Dataset_test.zip和Dataset_train.zip压缩包文件进行解压缩，放置在原data文件夹内；

（2）参考requirements.txt文件进行库安装；

（3）本文结果是在CPU为Inter E5-2680，内存为256G、 GPU为GeForce RTX 2080、操作系统为Ubuntu16.04.1的环境下得到的。

# 引用
如您在论文中使用了本项目代码，请引用：

王珏，洪敏轩，夏叶桐，徐秀钰，孔筱芳，万敏杰. 基于条件生成对抗网络的低照度彩色图像增强算法[J]. 红外与激光工程, 2024, 53(12): 1-13.
