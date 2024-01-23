# MMAlaya
MMAlaya是基于大语言模型[Alaya](https://github.com/DataCanvasIO/Alaya)的多模态模型。

MMAlaya包含以下三个模块：
<br>1，大语言模型Alaya。
<br>2，图像文本特征编码器来自[blip2-opt-2.7b](https://huggingface.co/Salesforce/blip2-opt-2.7b)的Qformer。
<br>3，图像文本特征到大预言模型的线性投影器。

模型的训练主要基于[LLaVA](https://github.com/haotian-liu/LLaVA)架构

2024.01.23 最终在[MMBench](https://mmbench.opencompass.org.cn)线上测试中文测试集分数为56.9，英文测试集分数为59.8。

推理可以参考 [inference.py](https://github.com/bingwork/MMAlaya/blob/inference/inference.py)