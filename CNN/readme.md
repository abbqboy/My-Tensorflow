# 卷积神经网络

 因为本人主要做的是医学图像处理，所以使用的主要是CNN

* 1、卷积

* 2、池化

* 3、全连接

* 4、梯度下降法

* 5、softmax

就以上5点对CNN做一个基本的介绍

![cnn](https://github.com/abbqboy/Sticker/blob/master/photo/cnn.png?raw=true)

## 神经网络的优化

* 1.学习率

训练神经网络，需要设置学习率（learning rate)控制参数更新的速度

学习率决定了参数每次更新的幅度

![xuexi](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1507182480251&di=c7858a239b906038e135380595e6a080&imgtype=0&src=http%3A%2F%2Fwww.aibosha.com%2Fdownloads%2Fimages%2F201701%2F1485250087881_5.png)

* 2.过拟合

模型不是尽量模拟训练数据的行为，而是希望通过训练出来的模型对未知数据给出判断

* 滑动平均模型

在Tensorflow中提供了tf.train.ExonentialMovingAverage来实现滑动平均模型





