# ArtMind_Flask

基于机器学习的绘画分析（风格，流派，情感，画家）和推荐系统
技术栈：Flask+Vue+Pytorch+Surprise

## Todos
1. 规范数据集命名方式
2. 验证多分类下的效果
1. 数据集扩充
2. 数据集备份
2. 更新前台页面交互逻辑
1. 考虑模型权重的应用调用问题
1. 更换建议的网络测试效果

## Archive

1. 搭建爬虫引擎，完成部分数据集的爬取
2. 整理形成西方绘画小规模数据集
3. 简单二层卷积神经网络模型的搭建
1. 分离训练和测试逻辑
2. 分离网络实现
3. 数据集加入伦勃朗，委拉斯凯兹，拉斐尔，鲁本斯的作品，扩充了具象数据集
4. 初步在目前的网络中训练了三分类（抽象 98、具象 198，意象 140）分类器的效果，20 epoches 下准确度来到了 88%
5. 在训练脚本中加入了可视化的内容
6. 加入卡拉瓦乔

## Problems

1. 目前的抽象选择的是极简主义，之前选择以达利和毕加索作品为主的超现实主义效果不佳
2. 目前训练集还是有点少，还是要扩充训练集
3. 目前的分类类别参数建议之后改为读取文件夹个数动态指定，或者写死在配置文件里面
4. 目前的抽象具象输出为单类别，我想要的是在这三个维度上面的概率，需要认真仔细分析一下