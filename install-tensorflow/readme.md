# Win7环境下使用Anaconda4.2安装Tensorflow

* Anaconda必须安装4.2版本，不能安装4.3版本
（因为我们需要安装自带的python必须是3.5，才可以调用TensorFlow。但是anaconda4.3自带是python3.6 ，无法调用TensorFlow ）
 


下面开始愉快的安装。
* 第一步：官网：https://www.continuum.io/downloads 目前官网是4.3 千万别手贱去下载
![anzhuang](https://github.com/abbqboy/My-Tensorflow/blob/master/install-tensorflow/photo/20170331104003073.png?raw=true)
![pp](

* 第二步：安装Anaconda
安装过程中，Anaconda会提示是否添加到环境变量，选择“是”；（其实不用太看，基本上一直next到底就好了）

* 第三步：检测python是否安装，环境配置是否成功
cmd 》》》python 
验证是否安装成功：

* 第四步：TensorFlow安装
以管理员身份运行cmd 
cd到这个地址：
补充信息： 
一键安装（CPU版）：

（GPU版）

* 第五步：测试

在cmd输入


第三坑：cmd进行Tensflow安装的时候，以管理员身份运行，进行安装。
