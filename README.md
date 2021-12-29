# PaddleOCR-Quicker
An GUI for PaddleOCR whl based on [Quicker](https://getquicker.net/).</br>
针对[PaddleOCR whl包](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.4/doc/doc_ch/quickstart.md)的可视化：通过可视化界面完成whl包不同参数的配置，实现截图后零命令使用whl包OCR识别功能。

## 1. 使用准备

### 1.1 [Python环境搭建](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.4/doc/doc_ch/environment.md)

### 1.2 [PaddleOCR whl包安装](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.4/doc/doc_ch/quickstart.md)

### 1.3 [Quicker安装](https://getquicker.net/)

本界面是基于软件[Quicker](https://getquicker.net/)的动作，适用平台**Windows**，功能实现参考Quicker内置`截图OCR`动作。

### 1.4 [安装动作](https://getquicker.net/kc/manual/doc/install-action)

安装Quicker后，在分享页面[PaddleOCR](https://getquicker.net/Sharedaction?code=5ebc2ab2-1325-449b-99b3-08d9c6b06ad1)点击**复制到剪贴板**，然后在Quicker界面空白处点击右键**粘贴分享的动作**。详细步骤可以参考Quicker官方文档[安装分享的动作](https://getquicker.net/kc/manual/doc/install-action)。

## 2. 使用介绍

### 2.1 第一次使用提示

第一次使用时，会提示需要安装PaddleOCR whl包。如果已安装，则会提示设置PaddleOCR所在环境；如果未安装，则会提示` 1.2 PaddleOCR whl包安装 `的教程网页。

### 2.2 无文本窗口模式

截图后不弹出文本编辑窗口，只弹出简单的消息提示。OCR识别的结果会自动复制到剪贴板。

### 2.3 文本窗口模式

截图后弹出文本编辑窗口，可以在文本编辑窗口中，用`段落处理`和`标点处理`功能进行简单的文字处理。OCR识别的结果不会自动复制到剪贴板。

### 2.4 设置选项

设置选项可以在PaddleOCR动作图标上单击右键呼出。主要有`文本窗口模式设置`、`识别设置`和`环境设置`三处。

## 3. 前实现功能

### 3.1 设置语言

默认设置为`--lang=ch`，目前支持10种语言中英文、英语、中文繁体、日语、韩语、法语、西班牙语、德语、意大利语、俄语

### 3.2 设置是否启用GPU

默认设置为`--use_gpu false`

### 3.3 设置是否启用方向分类器

默认设置为`--use_angle_cls true`，开启可识别180度旋转文字

### 3.4 文本处理功能

文本处理功能，主要分`段落处理`和`标点处理`两个模块，均源自`截图OCR`动作

### 3.5 设置截图后是否显示文本窗口

在PaddleOCR动作图标上单击右键，可以看到`开启\关闭 文本窗口显示`的选项，关闭后OCR识别结果直接复制到剪贴板。

## TODO

- [ ] 增加识别置信度解析，并可视化
- [ ] 增加可选参数——单独使用检测`--rec false`
- [ ] 增加可选参数——单独使用识别`--det false`
- [ ] 增加可选参数——版面分析`--type=structure`，并解析结果
