# MMAlaya
MMAlaya是基于大语言模型[Alaya](https://github.com/DataCanvasIO/Alaya)的多模态模型，模型权重文件在[DataCanvas/MMAlaya](https://huggingface.co/DataCanvas/MMAlaya/tree/main)

MMAlaya包含以下三个模块：
<br>1，大语言模型[Alaya-7B-Chat](https://huggingface.co/DataCanvas/Alaya-7B-Chat)。
<br>2，图像文本特征编码器来自[blip2-opt-2.7b](https://huggingface.co/Salesforce/blip2-opt-2.7b)的EVA-G。
<br>3，图像文本特征到大预言模型的连接器,使用的是来自[blip2-opt-2.7b](https://huggingface.co/Salesforce/blip2-opt-2.7b)的Qformer和线性投影器。

模型的训练主要基于[LLaVA](https://github.com/haotian-liu/LLaVA)架构

OpenCompass 评测榜单，均分41.1，排名25名。
![opencompass-leaderboard-multimodal](https://github.com/DataCanvasIO/MMAlaya/blob/main/data/opencompass-leaderboard-multimodal.png)
MMBench 评测榜单，开源开放的模型，中文测试集，均分58.6，排名25名。
![opencompass-leaderboard-multimodal-cn](https://github.com/DataCanvasIO/MMAlaya/blob/main/data/opencompass-leaderboard-multimodal-cn.png)

推理可以参考 [inference.py](https://github.com/DataCanvasIO/MMAlaya/blob/main/inference.py)
请使用transformers==4.33.0，否则会报错ImportError: cannot import name '_expand_mask' from 'transformers.models.bloom.modeling_bloom'。

# Citation
MMAlaya使用<a href="https://github.com/DataCanvasIO/Alaya/blob/main/LICENSE">Apache 2.0 Lisense</a>，开放模型权重，允许商业用途。如果您的项目引用了我们的MMAlaya，请标明出处，并点个小星星 :star: ：
```
@misc{datacanvas2024mmalaya,
    author = {DataCanvas Ltd.},
    title = {mmalaya},
    year = {2024},
    howpublished = {\url{https://github.com/DataCanvasIO/MMAlaya}},
}
```
