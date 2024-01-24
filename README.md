# 新闻推荐系统

这个代码实现了neural news recommendation with attentive multi-view learning新闻推荐系统模型，即注意力多试图的神经新闻推荐系统

| 模型   | 全称                | 论文                               |
| ---- | ----------------- | -------------------------------- |
| NAML | 基于注意力多试图学习的神经新闻推荐 | https://arxiv.org/abs/1907.05576 |

运行代码之前需要下载glove预训练嵌入

```
wget https:/nlp.stanford.edu/data/glove.8408.300d.zip
```

下载微软官方MIND数据集

```
https://mind20191smallblob.core.windows.net/release/MINDLarge_train.zip
https://mind20191osmall.blob.core.windows.net/release/MINDlarge_test.zip
https://mind20191osmall.blob.core.windows.net/release/MINDLarge_dev.zip
```

先进行数据预处理

```
python src/data_preprocess.py
```

运行

```
python src/train.py
python src/evaluate.py
```
