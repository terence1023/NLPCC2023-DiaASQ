# NLPCC-Share-Task4 HLT-base

- NLPCC-Share-Task4 Conversational Aspect-based Sentiment Quadruple Analysis Top 2.

## 准备
运行前需要下载预训练语言模型到`project/pre_trained_model`目录下，详细见`project/pre_trained_model/README.md`文件

## train
```
sh train.sh
```
训练好的权重会保存在`project/data/save/current_timestamp`文件夹下，其中`current_timestamp`表示当前运行的时间戳。在训练完成后，会自动加载最好的dev结果对应的权重文件，生成预测结果。


## test
```
sh test.sh
```
比赛提交结果使用的权重路径分别是：
- 中文：`project/save/zh_14.pth.tar`
- 英文：`project/save/en_14.pth.tar`


## 运行环境

```
V100-32G
```


