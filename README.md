# PaddleOCR-Quicker
GUI for PaddleOCR whl based on Quicker
针对PaddleOCR whl包的可视化：通过可视化界面完成whl包不同参数的配置，实现截图后零命令使用whl包OCR识别功能
## 1.使用须知
1. 本界面是基于软件[Quicker](https://getquicker.net/)的动作，适用平台**Windows**。安装Quicker后，在分享页面[PaddleOCR](https://getquicker.net/Sharedaction?code=5ebc2ab2-1325-449b-99b3-08d9c6b06ad1)点击**复制到剪贴板**，然后在Quicker界面空白处点击右键**粘贴分享的动作**。
2. 第一次使用时会有使用提示，按照[PaddleOCR官方仓库](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.4/doc/doc_ch/quickstart.md)教程，完成PaddleOCR whl包安装。

## 2.目前实现功能
![image](https://user-images.githubusercontent.com/27466624/147352331-2a851fe3-aec7-4afd-bac3-99df5fe2a4b6.png)
1. 更改语言设置`--lang=ch`，目前支持10中语言；
2. 调整是否启用GPU`--use_gpu false`
3. 调整是否启用方向分类器识别180度旋转文字`--use_angle_cls true`

## TODO
