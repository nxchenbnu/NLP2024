# Assignment-1 Word2Vec

## 环境配置
首先请大家安装好anaconda，完成后继续以下内容。

创建环境，用env.yml:
    
    conda env create -f env.yml

激活环境:

    conda activate nlpclass

在nlpclass中安装(示例) pytorch https://pytorch.org/get-started/locally/
    
    conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia

## 任务描述：

目标： 使用NLTK库中的Reuters (business and financial news) corpus语料库，基于Word2Vec的Skip-gram模型，使用PyTorch实现词向量的训练。

要求： 训练完成后，能够查询词语的相似度，并对词向量进行可视化展示。

## 具体要求：

1. 数据预处理：加载Reuters语料库，对文本进行清洗和分词处理。

2. 构建词汇表，过滤低频词（如词频小于5），为每个单词分配唯一的索引。

3. 构建训练数据：使用Skip-gram模型，生成中心词和上下文词对。

4. 实现负采样（Negative Sampling）策略，生成负样本。

5. 模型构建：使用PyTorch构建Word2Vec模型，包括嵌入层和输出层。

6. 实现自定义的损失函数，如负采样损失（Negative Sampling Loss）。

7. 模型训练：设置合适的超参数（如嵌入维度、学习率、批次大小、训练轮数等）。选择合适的优化器（如SGD或Adam）进行模型训练。

8. 结果评估与可视化：计算词语之间的余弦相似度，展示某些词的最相似词列表。使用t-SNE或PCA对词向量进行降维，并进行可视化。

## 作业提交：
代码部分：提交完整的Python代码，代码应有清晰的注释和说明。

报告部分：1. 简要说明实现过程，包括遇到的问题和解决方案。 2.展示训练结果和可视化图表，对结果进行分析和讨论。3. 回答最后提出的三个问题。