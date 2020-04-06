# tf_predicate
通过 tensorflow 预测房屋价格趋势（租房数据）

步骤:
import 所需包数据
```
# coding: utf-8
import tensorflow as tf
from sklearn.datasets import load_boston
import matplotlib.pyplot as plt
from sklearn.preprocessing import scale
from sklearn.model_selection import train_test_split
```

获取数据并将数据清理降维和归一化 标准化
目前从六个维度输入预测价格输出数据

城市，区域，小区，面积 ，朝向，户型 


创建训练集与测试集
（涉及数据网盘下载）

选择不同的算法对数据集进行预测

算法1:
  线性回归
   线性回归的主要思想是通过历史数据拟合出一条直线，因变量与自变量是线性关系，对新的数据用这条直线进行预测。
   
   模型评估
   ```
   print("模型训练集的准确率：%.3f" %lr.score(x_train, y_train))
   print("模型测试集的准确率：%.3f" %lr.score(x_test, y_test))
   ```
   可视化预测结果数据


