# 202106wechat_alog
比赛时间2021.6  
名次：未进复赛，300名左右  
官网地址：https://algo.weixin.qq.com/  
自我评价：意料之中的成绩，第一次参加这种推荐算法类比赛，技术不够成熟，很多关键上分点未能复现。如果再刻苦一点兴许可以突破自我。  
1.lgb部分收获   
1）生成特征，对id之间做embbedding，生成N位向量作为新的特征。大概能提升1%  
2）tfdif，对无需的数做处理生成N维向量  
3）7天&5天滑窗，详见baseline，通过滑窗生成特征能提升不小分数。  
4）PCA降维，可以把复杂的数降维成64位/16位，再merge作为特征  
5）多任务训练，即需要预测多个指标时，循环生成多个预测结果  
2.nn部分收获  
1）deepfm算法原理与基础bseline  
2）深度学习的包调用逻辑  
3.需要提升的地方（后续学习优秀团队代码）  
1）周榜中多次提到keywords&tag，可这个具体应该怎么做呢？  
2）embedding特征如何更好处理。我是抄了华为赛的embbeding，效果一般。需学习大佬如何embeding  
3）深度学习中din与mmoe。这两个模型据说很好用，可是我能力不足无法复现  
4.遗憾  
1）B榜没留足够的时间。以前比赛B榜数据集和A榜一致，无需重跑。此次比赛需重跑，所以应发B榜时就跑起来以便后续之用。  
2）lgb没有和上次熟悉的auto-ml结合，不够好  
3）没使用cbt融合  

代码部分是我加了tfdif，embedding的lgb，与baseline的deepfm，以便后续学习
