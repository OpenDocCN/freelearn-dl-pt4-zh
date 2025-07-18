# 序言

你曾经尝试过让计算机做出一些新颖的事情吗？我可以让你编写一个故事，或者看一张图片并告诉我其中的内容。你如何让计算机程序像这样表现，而不是像过去 30 多年我们所使用的数字存储和传输单元呢？

如果你拥有完美的知识和无限的时间，你可以编写出计算机程序所需遵循的所有规则。当然，如果你有足够的知识来定义操作规则，那么你就不需要计算机来做任何事情了！那么，当你需要计算机以复杂的方式运作（进行预测、分类、优化过程、生成内容、响应交互、执行机器人控制）但又没有完全定义所有启发式规则时，你该怎么办呢？

你构建一个基于算法的应用程序，能够从相关领域的数据中学习规则、寻找模式或确定信号。你设定训练过程，使其能够以极快的速度进行迭代，且进行大量循环（我们称之为 epochs），以提供“经验”，从而在一个人类寿命内无法完成的过程中逐步训练模型。

当我们将这些算法架构分层构建时，我们创造了能够学习特征的深度学习模型（例如，狗有尾巴，车有轮子），而这些学习到的特征是非常强大的！我们在《*Python 深度学习项目*》中真正发现的是，我们能够提出之前无法回答的深刻问题。正是这些问题推动了深度学习技术解决从放射学中的医疗诊断到癌症筛查等问题。深度学习应用推动了聊天机器人体验、人脸识别、自动驾驶、推荐引擎和营销技术的发展。物理学、生物学和化学的硬科学也在将深度学习技能训练纳入其中，正如过去对统计学和显微镜的应用一样。

# 本书适合人群

如果你已经学习过至少一门机器学习课程，并且具备一定的 Python 使用能力（意味着在示例支持下，你可以用 Python 编写程序），那么本书非常适合你。我们的许多读者将是学习计算机科学、统计学、数学、物理学、生物学、化学、市场营销和商业等专业的本科生。深度学习技术正在应用于这些学位所为你准备的所有职业，而本书是学习这些技能的绝佳方式，这些技能将直接有助于你的成功。研究生们也会很喜欢这本书的教学水平，因为所选的项目直接适用于现代职场，从科技初创公司到企业应用。

*Python 深度学习项目* 聚焦于数据科学管道的核心——模型构建、训练、评估和验证。由于篇幅限制，数据管道中生产应用所需的额外前期和后期数据工程过程在此无法详细讨论，但我们计划在未来的出版物中进行探讨。

# 本书内容概览

第一章，*构建深度学习环境*，在本章中，我们将建立一个通用的工作空间，包含核心技术，如 Ubuntu、Anaconda、Python、TensorFlow、Keras 和 **Google Cloud Platform** (**GCP**)。

第二章，*使用回归训练神经网络进行预测*，在本章中，我们将在 TensorFlow 中构建一个 2 层（最小深度）神经网络，并使用经典的 MNIST 手写数字数据集对其进行训练，应用于餐厅顾客短信通知业务案例。

第三章，*使用 word2vec 进行词表示*，在本章中，我们将学习并使用 word2vec 将词转换为稠密向量（即张量），为语料库创建嵌入表示，然后构建 **卷积神经网络** (**CNN**) 来为情感分析构建语言模型，应用于文本交换业务案例。

第四章，*构建用于聊天机器人的 NLP 流水线*，在本章中，我们将创建一个 NLP 流水线，对语料库进行分词、标注词性、通过依赖解析确定词之间的关系，并进行命名实体识别（NER）。使用 TF-IDF 对文档中的特征进行向量化，创建一个简单的 FAQ 类型聊天机器人。通过命名实体识别（NER）和 Rasa NLU 实现来增强此聊天机器人，使其能够理解上下文（意图），提供准确的响应。

第五章，*用于构建聊天机器人的序列到序列模型*，在本章中，我们将使用 [第四章](https://cdp.packtpub.com/python_deep_learning_projects/wp-admin/post.php?post=727&action=edit#post_27)，*构建用于聊天机器人的 NLP 流水线*，聊天机器人来构建一个更为先进的聊天机器人，结合早期项目中的学习，使用多种技术使其更具上下文感知能力和鲁棒性。我们通过构建 **递归神经网络** (**RNN**) 模型，并结合 **长短期记忆** (**LSTM**) 单元，避免了 CNN 在聊天机器人中存在的一些局限性，LSTM 专门用于捕捉字符或单词序列中表示的信号。

第六章，*内容创作的生成性语言模型*，在本章中，我们实现一个生成性模型，使用**长短期记忆网络**（**LSTM**）、变分自编码器和**生成对抗网络**（**GANs**）生成内容。你将有效地实现文本和音乐的模型，能够为艺术家和各种创意企业生成歌曲歌词、剧本和音乐。

第七章，*使用 DeepSpeech2 构建语音识别*，在本章中，我们将构建并训练一个**自动语音识别**（**ASR**）系统，该系统接受音频通话并将其转换为文本，然后可以将文本作为输入用于基于文本的聊天机器人。通过处理语音和声谱图，构建一个端到端的语音识别系统，并使用**连接时序分类**（**CTC**）损失函数、批量归一化和 SortaGrad 进行 RNN 训练。本章是《*Python 深度学习项目*》书中自然语言处理部分的核心章节。

第八章，*使用 ConvNets 进行手写数字分类*，在本章中，我们将教授**卷积神经网络**（**ConvNets**）的基础知识，重点讨论卷积操作、池化和丢弃正则化。这些是你在职业生涯中调节模型时需要掌握的工具。与第二章中*使用回归训练神经网络进行预测*的早期*Python 深度学习项目*相比，你将看到部署更复杂、更深层模型在性能上的价值。

第九章，*使用 OpenCV 和 TensorFlow 进行目标检测*，在本章中，我们将学习如何掌握目标检测和分类，并使用比之前项目更为信息复杂的数据，来产生令人印象深刻的结果。学习使用深度学习包 YOLOv2，并获得该模型架构如何变得更加深入复杂并取得良好效果的经验。

第十章，*使用 FaceNet 构建人脸识别*，在本章中，我们将使用 FaceNet 构建一个模型，该模型查看一张图片并识别其中的所有可能面孔，然后执行人脸提取以了解图像中人脸部分的质量。对图像中已识别人脸部分进行特征提取，为与另一个数据点（该人的标注面孔图像）进行比较提供基础。这个*Python 深度学习项目*展示了该技术在从社交媒体到安全等应用中的激动人心的潜力。

第十一章，*自动图像描述生成*，在本章中，我们将结合到目前为止在*Python 深度学习项目*中学到的最前沿技术，涵盖*计算机视觉*和*自然语言处理*，构建一个完整的图像描述方法。实现这一目标的聪明方法是将编码器-解码器架构中的编码器（RNN 层）替换为一个经过训练的深度**卷积神经网络**（**CNN**），该网络能够对图像中的物体进行分类。这个模型能够生成任何提供图像的计算机生成自然语言描述。

第十二章，*使用卷积神经网络在 3D 模型中进行姿势估计*，在本章中，我们将在 Keras 中成功构建一个深度卷积神经网络/VGG16 模型，应用于**电影标签图像**（**FLIC**）。获得实际操作经验，了解如何准备图像以进行建模。成功实施迁移学习，并测试修改后的 VGG16 模型在未见数据上的表现，以确定是否成功。

第十三章，*使用 GAN 进行图像翻译与风格迁移*，在本章中，你将构建一个神经网络，填补手写数字的缺失部分。重点放在模型的创建——利用 GAN 进行神经修复（生成/重构）手写数字的缺失部分，随后你将重新构建（生成回）缺失的部分，使分类器能够接收到清晰的手写数字，以便转换成数字。

第十四章，*使用深度强化学习开发自主智能体*，在本章中，我们将构建一个深度强化学习模型，成功玩转 OpenAI Gym 中的 CartPole-v1 游戏。学习并展示在 Gym 工具包中的专业能力，掌握 Q 学习与 SARSA 学习，如何编码强化学习模型并定义超参数，构建训练循环并测试模型。

第十五章，*总结与你深度学习职业的下一步*，在本章中，你将回顾关键学习内容，总结深度学习项目的直觉，并展望你深度学习职业生涯的下一步。

# 充分利用本书的内容

我们从一个非常实际的角度来处理深度学习项目。在思考如何分享我们的知识、经验、所学策略和我们采用的战术时，将这本书格式化成这样似乎是自然而然的——你（读者）仿佛是我们“智能工厂”应用 AI 工程团队的一员。

为了从这些项目中获得最大的收获，你至少需要具备基本的 Python 工作知识，并且对深度学习概念有所了解。本书《Python 深度学习项目》主要是一本技术性指导书，内容涉及深度学习的直觉方面，以帮助你学习能产生实际工作的模型代码。本书不涉及深度探讨作为这些技术基础的微积分。

每一章就像是参与 AI 团队的每周站会。当你与这些内容互动时，你将会：

+   看清整体大局

    +   这个项目的实际应用案例和目标是什么？

    +   成功的影响是什么？

    +   我们的战略是什么，如何实现目标？

+   集中精力，开始编写代码吧！

    +   确定实现项目目标的具体策略

    +   为什么这是正确的方法？

    +   反复执行这些策略

        +   输入或建立背景是什么？

        +   代码示例

        +   输出和成功标准

    +   问答环节

        +   我们有什么问题？

        +   你可能会有哪些问题？

+   再次回到整体大局

    +   让我们确认是否达成了目标

    +   从这段经历中我们能获得什么直觉？

    +   如何将这一成功经验推广到新的应用场景？

解释 Python 深度学习就像 1-2-3 一样简单！但是，讨论深度学习并不等同于实际操作，而这正是本书的主题。接下来将展示一些发人深思且令人兴奋的经历。我们将使用最先进的 Python 库和技术，赋能你（我们最新的应用 AI 工程团队成员），让你能通过本书中创建的项目为你的职业生涯做出贡献。我们很高兴你能参加我们每周的 AI 团队站会。

现在让我们一起学习，享受其中的乐趣，并在这些 Python 深度学习项目中做出出色的工作！

# 下载示例代码文件

你可以从你的账户在[www.packt.com](http://www.packt.com)下载本书的示例代码文件。如果你在其他地方购买了本书，可以访问[www.packt.com/support](http://www.packt.com/support)，并注册以便直接将文件通过电子邮件发送给你。

你可以按照以下步骤下载代码文件：

1.  登录或注册 [www.packt.com](http://www.packt.com)。

1.  选择 SUPPORT 标签。

1.  点击代码下载和勘误表。

1.  在搜索框中输入书名，并按照屏幕上的指示操作。

一旦文件下载完成，请确保使用最新版本的以下工具解压或提取文件夹：

+   WinRAR/7-Zip for Windows

+   Zipeg/iZip/UnRarX for Mac

+   7-Zip/PeaZip for Linux

本书的代码包也托管在 GitHub 上，地址为[**https://github.com/PacktPublishing/Python-Deep-Learning-Projects**](https://github.com/PacktPublishing/Python-Deep-Learning-Projects)。如果代码有更新，将会在现有的 GitHub 仓库中进行更新。

我们还在我们丰富的书籍和视频目录中提供了其他代码包，您可以在 **[`github.com/PacktPublishing/`](https://github.com/PacktPublishing/)** 查阅它们！快来看看吧！

# 下载彩色图像

我们还提供了一个 PDF 文件，其中包含本书中使用的截图/图表的彩色图像。您可以在此下载：[`www.packtpub.com/sites/default/files/downloads/9781788997096_ColorImages.pdf`](http://www.packtpub.com/sites/default/files/downloads/9781788997096_ColorImages.pdf)。

# 使用的约定

本书中使用了许多文本约定。

`CodeInText`：表示文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟网址、用户输入以及 Twitter 账号。例如：“一旦您安装了 Docker，您应该能够在终端使用 `docker` 命令。”

代码块如下所示：

```py
import sys
import dlib
from skimage import io
```

当我们希望特别引起您对代码块中特定部分的注意时，相关的行或项目会以粗体显示：

```py
# Create a HOG face detector using the built-in dlib class
face_detector = dlib.get_frontal_face_detector()
```

任何命令行的输入或输出如下所示：

```py
curl https://get.docker.com | sh
```

警告或重要提示如下所示。

提示和技巧如下所示。

# 联系我们

我们始终欢迎读者的反馈。

**一般反馈**：如果您对本书的任何内容有疑问，请在邮件的主题中提及书名，并通过电子邮件联系我们：`customercare@packtpub.com`。

**勘误**：虽然我们已经尽力确保内容的准确性，但错误仍然可能发生。如果您在本书中发现了错误，我们将非常感激您向我们报告。请访问 [www.packt.com/submit-errata](http://www.packt.com/submit-errata)，选择您的书籍，点击“勘误提交表单”链接，并输入详细信息。

**盗版**：如果您在互联网上发现任何非法复制的我们作品的形式，我们将非常感激您提供该位置或网站名称。请通过 `copyright@packt.com` 联系我们，并提供该材料的链接。

**如果您有兴趣成为作者**：如果您在某个领域有专业知识，并且有兴趣撰写或贡献书籍，请访问 [authors.packtpub.com](http://authors.packtpub.com/)。

# 评论

请留下评论。阅读并使用本书后，您不妨在购买网站上留下评论。潜在读者可以参考您的公正意见来做出购买决定，我们 Packt 可以了解您对我们产品的看法，作者也能看到您对其书籍的反馈。感谢您！

如需了解更多关于 Packt 的信息，请访问 [packt.com](http://www.packt.com/)。
