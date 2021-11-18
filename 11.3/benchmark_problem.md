# 果蝇数据实验中出现的问题

## 实验描述

TEtranscript（2015）文献中使用4个工具对果蝇数据进行了转座元件表达量的对比实验，并且使用的数据使用了QPCR进行转座元件的准确定量

![image-20211117164900021](https://tva1.sinaimg.cn/large/008i3skNly1gwi8tx38lzj30zt0neq4u.jpg)

横轴是8种果蝇基因组中的转座元件，纵轴是实验组与对照组转座元件表达量的log2FC值，数值越高则差异越大。

## 遇见问题

### 1. 转座元件类型

在repeatmasker下载了果蝇的转座元件注释文件。

以MDG1为例，注释文件中包含了MDG1_LTR和MDG1_I-int两种，然后文献也没写具体用的是哪个还是两个加起来。

![image-20211117170236705](https://tva1.sinaimg.cn/large/008i3skNly1gwi9832rbcj323k07aad9.jpg)

### 2. 其它的具体数值

没有在supplementary文件中找到这个直方图的具体数值，不知道如何重画这个直方图。

## 结果

![直方图（新增）](https://tva1.sinaimg.cn/large/008i3skNly1gwh5h4thn2j30rs0jgta0.jpg)

其中使用的都是例如MDG1_I-int、DM297_I-int的数据，而MDG_LTR等数据没有I-int数据准确。I-element不知道是什么转座元件。

