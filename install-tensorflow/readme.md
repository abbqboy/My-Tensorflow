# Win7环境下使用Anaconda4.2安装Tensorflow

* Anaconda必须安装4.2版本，不能安装4.3版本
（因为我们需要安装自带的python必须是3.5，才可以调用TensorFlow。但是anaconda4.3自带是python3.6 ，无法调用TensorFlow ）
 


下面开始愉快的安装。
* 第一步：官网：https://www.continuum.io/downloads 目前官网是4.3 千万别手贱去下载
![anzhuang](https://github.com/abbqboy/My-Tensorflow/blob/master/install-tensorflow/photo/20170331104003073.png?raw=true)
![pp](https://github.com/abbqboy/My-Tensorflow/blob/master/install-tensorflow/photo/1111.png?raw=true)

* 第二步：安装Anaconda
安装过程中，Anaconda会提示是否添加到环境变量，选择“是”；（其实不用太看，基本上一直next到底就好了）

* 第三步：检测python是否安装，环境配置是否成功

cmd>>python 验证是否安装成功：

![1111](https://github.com/abbqboy/My-Tensorflow/blob/master/install-tensorflow/photo/2222.png?raw=true)

* 第四步：TensorFlow安装

以管理员身份运行cmd 

cd到这个地址：cd Program Files\Anaconda3\Scripts 

补充信息：

一键安装（CPU版）：pip install --upgrade --ignore-installed tensorflow
相关知识插入：TensorFlow 有两个版本：CPU 版本和 GPU 版本。GPU 版本需要 CUDA 和 cuDNN 的支持，CPU 版本不需要。

如果你要安装 GPU 版本，请先确认你的显卡支持 CUDA。


1.确认版本：pip版本 >= 8.1。用 pip -V 查看当前 pip 版本，用 python -m pip install -U pip 升级pip 

2.确保你安装了 VS2015 或者 2013 或者 2010。

（GPU版）：pip install --upgrade --ignore-installed tensorflow-gpu

* 第五步：测试

在cmd输入python

>>import tensorflow as tf

>>hello = tf.constant('Hello, TensorFlow!')

>>sess = tf.Session()

>>print(sess.run(hello))

输出：Hello, TensorFlow!

输入：

>>a = tf.constant(10)

>>b = tf.constant(32)

>>print(sess.run(a + b))

输出：42(说明TensorFlow安装完成）

本人用的IDE是Anaconda自带的Spyer

