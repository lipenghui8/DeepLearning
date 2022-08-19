# 整体结构

![image-20220819095852862](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819095852862.png)

- 特征提取器，分类器

## 卷积

![image-20220819102718670](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819102718670.png)

![image-20220819104334982](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819104334982.png)



### 卷积核的通道数由输入的通道数决定，输出的特征图数量由卷积核的数量决定

![image-20220819104556071](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819104556071.png)

![image-20220819104825276](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819104825276.png)

- 权重就是这四个维度

## 代码实现

![image-20220819105435595](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819105435595.png)

- 需要确定输入通道，输出通道以及卷积核大小

- padding:在图像的外围添加几圈0，根据需求决定添加几圈

![image-20220819110206438](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819110206438.png)

### 步长（卷积核一次移动几格）

![image-20220819110317154](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819110317154.png)

![image-20220819111848834](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819111848834.png)

## 最大池化（默认步长为2，降采样，通道不变）

![image-20220819112134441](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819112134441.png)

![image-20220819112211502](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819112211502.png)

![image-20220819112910093](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819112910093.png)

![image-20220819113359615](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819113359615.png)

### 使用GPU

![image-20220819113748382](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819113748382.png)

![image-20220819113850076](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819113850076.png)

- 模型和数据要在同一块显卡上

![image-20220819113944039](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220819113944039.png)