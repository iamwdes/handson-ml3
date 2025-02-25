机器学习笔记本，第三版
================================

该项目旨在教您用Python掌握机器学习。它包含了我的O'Reilly书 [使用Scikit-Learn，Keras和Tensorflow（第3版）的第三版中的练习的示例代码和解决方案](https://homl.info/er3)：

<a href="https://homl.info/er3"><img src="https://learning.oreilly.com/library/cover/9781098125967/300w/" title="book" width="150" border="0" /></a>

**Note**：如果您正在寻找第二版笔记本电脑，请查看 [AGERON/HANDSON-ML2](https://github.com/ageron/handson-ml2)。有关第一版，请参见 [AGERON/HANDSON-ML](https://github.com/ageron/handson-ml)。

## 快速开始

### 想要在线玩这些笔记本，而不必安装任何东西？

* <a href="https://colab.research.google.com/github/ageron/handson-ml3/blob/main/" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>（推荐）

⚠_colab提供了一个临时环境：一段时间后您所做的任何事情都将被删除，因此请确保下载您关心的所有数据。

<details>

其他服务也可能起作用，但我尚未完全测试它们：
* <a href="https://homl.info/kaggle3/"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open in Kaggle" /></a>

* <a href="https://mybinder.org/v2/gh/ageron/handson-ml3/HEAD?filepath=%2Findex.ipynb"><img src="https://mybinder.org/badge_logo.svg" alt="Launch binder" /></a>
* <a href="https://homl.info/deepnote3/"><img src="https://deepnote.com/buttons/launch-in-deepnote-small.svg" alt="Launch in Deepnote" /></a>

</details>

### 只想快速查看一些笔记本，而无需执行任何代码？

* <a href="https://nbviewer.jupyter.org/github/ageron/handson-ml3/blob/main/index.ipynb"><img src="https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg" alt="Render nbviewer" /></a>
* [github.com的笔记本查看器](https://github.com/ageron/handson-ml3/blob/main/index.ipynb)也有效，但它并不理想：它很慢，数学方程并不总是显示正确的是，大型笔记本电脑通常无法打开。

### 想使用Docker图像运行此项目？
阅读 [Docker指令](https://github.com/ageron/handson-ml3/tree/main/main/docker)。

### 想在您自己的计算机上安装此项目吗？

首先安装 [Anaconda](https://www.anaconda.com/products/distribution)（或 [Miniconda](https://docs.conda.io/en/en/latest/miniconda.html))，[git](https://git-scm.com/downloads)，如果您有TensorFlow兼容GPU，安装 [GPU驱动程序 ](https://www.nvidia.com/download/index.aspx)，以及适当的Cuda和Cudnn（有关更多详细信息）的适当版本的Cuda和Cudnn（请参阅Tensorflow的文档）。

接下来，通过打开终端并键入以下命令来克隆此项目（请勿键入第一个`$`）:

    $ git clone https://github.com/ageron/handson-ml3.git
    $ cd handson-ml3

接下来,运行下面的命令：

    $ conda env create -f environment.yml
    $ conda activate homl3
    $ Python -M ipykernel install -user -name = python33

最后，启动jupyter：

    $ jupyter notebook

如果需要进一步的说明，请阅读[详细的安装说明](install.md)。

# 常问问题

**我应该使用哪个Python版本？**

我建议Python 3.10。如果您遵循上面的安装说明，那就是您将获得的版本。任何版本≥3.7也应起作用。

**调用`load_housing_data（）`** 时会遇到错误

如果您遇到了HTTP错误，请确保运行与笔记本中完全相同的代码（如果需要，请复制/粘贴）。如果问题仍然存在，请检查您的网络配置。如果是SSL错误，请参见下一个问题。

**我在MacOSX** 上遇到了SSL错误

您可能需要安装SSL证书（请参阅此[Stackoverflow问题](https://stackoverflow.com/questions/27835619/urllib-and-ssl-ssl-certificate-verify-verify-failed-error)）。如果您从官方网站下载了Python，请在终端中运行`/Applications/Python\ 3.10/Install\ Certificates.command`（将3.10更改为您安装的任何版本）。如果使用Macports安装Python，请在终端中运行`sudo port install curl-ca-bundle`。

**我已经在本地安装了该项目。如何将其更新为最新版本？**

请参阅[install.md](install.md)

**使用Anaconda时，如何将我的Python库更新为最新版本？**

请参阅[install.md](install.md)

## 贡献者
我要感谢所有[支持本项目的人](https://github.com/ageron/handson-ml3/contributors)，要么通过提供有用的反馈，提交提交问题或提交拉取请求。特别感谢Haesun Park和Ian Beauregard审查了每个笔记本并提交了许多PR，包括一些练习解决方案的帮助。还要感谢创建了'Docker'目录的Steven Bunkley和Ziembla，并感谢Github用户Superyorio为某些锻炼解决方案提供了帮助。非常感谢Victor Khaustov提交了许多出色的PR，解决了许多错误。最后，感谢Google ML开发人员计划团队，他们通过提供Google Cloud信用来支持这项工作。
