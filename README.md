# 项目介绍

该项目是为了自己训练一个"网络安全知识助手"模型，包括预训练、微调和RLHF等一系列步骤，后续会一直更新，并且每一步的数据、代码和权重都会上传。

大体步骤为：

1. 数据获取
2. 数据筛选
3. 数据打分
4. 选择合适的架构
5. 训练pre-train模型
6. 模型微调
7. benchmark
8. RLHF





# 数据打分

因为中文数据打分的模型、数据集太少了，因此用了10w的中文+10w的英文 全量微调了bert-base-chinese模型，

| 语言       | 模型              | 测试集正确率 |
| ---------- | ----------------- | ------------ |
| 中文       | bert-base-chinese | 0.8          |
| 中文       | xlm-roberta-large | 0.80         |
| 英文       | bert-base-uncase  | 0.6          |
| 英文       | xlm-roberta-large | 0.49         |
| 中英文混合 | xlm-roberta-large | 0.4          |
| 中英文混合 | bert-base-chinese | 0.68         |

模型地址为：https://huggingface.co/victcn/chinese_data_quality_score



后续会更新更多的内容..... 
