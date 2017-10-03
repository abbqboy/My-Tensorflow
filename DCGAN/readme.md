# 利用CIFAR-10数据实现DCGAN

## GAN（生成对抗网络）

从监督学习向半监督学习过渡

GAN是14年首次提出，其结构主要包括了两个部分

* 生成器Generator
* 判别器Discriminator

生成器主要用来学习真实图像分布从而让自身生成的图像更加真实，以骗过判别器。

判别器则需要对接收的图片进行真假判别。

在整个过程中，生成器努力地让生成的图像更加真实，而判别器则努力地去识别出图像的真假，这个过程相当于一个二人博弈，随着时间的推移，生成器和判别器在不断地进行对抗，最终两个网络达到了一个动态均衡

生成器生成的图像接近于真实图像分布，而判别器识别不出真假图像，对于给定图像的预测为真的概率基本接近0.5（相当于随机猜测类别）。

其自诞生以来发展的是相当火热，本文将以DCGAN为例进行实现。

![hei](https://github.com/abbqboy/Sticker/blob/master/photo/DAGAN/1.png?raw=true)

![ssss](https://github.com/abbqboy/Sticker/blob/master/photo/DAGAN/12.png?raw=true)

![hssei](https://github.com/abbqboy/Sticker/blob/master/photo/DAGAN/38.png?raw=true)












