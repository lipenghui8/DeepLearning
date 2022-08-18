## 梯度下降算法
![image-20220811120858931](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220811120858931.png)

## 随机梯度下降

![image-20220811153021180](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220811153021180.png)

![image-20220811154805263](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220811154805263.png)

## 简单线性模型的误差反向传播

![image-20220813105743414](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220813105743414.png)

- sgd:随机梯度下降的优化器
  
## pytorch  结构

![image-20220813112252736](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220813112252736.png)

## 损失函数与优化器构造

![image-20220813154725197](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220813154725197.png)

## 常用优化函数

![image-20220813163407854](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220813163407854.png)

常见希腊字母：

![img](https://iknow-pic.cdn.bcebos.com/6609c93d70cf3bc7efb7ba37df00baa1cc112ab1?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_600%2Ch_800%2Climit_1%2Fquality%2Cq_85%2Fformat%2Cf_auto)

### BCE Loss

![image-20220818160726495](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818160726495.png)

![image-20220818160755784](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818160755784.png)

![image-20220818174429879](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818174429879.png)

#### 激活函数

![image-20220818174658547](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818174658547.png)

![image-20220818175449467](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818175449467.png)

#### 基本定义

![image-20220818180055859](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818180055859.png)

- Shuffle：将数据集打乱顺序，之后再分组

![image-20220818185321376](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818185321376.png)

- num_workers：读取数据时设置几个线程并行

![image-20220818185537048](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818185537048.png)

#### 加载数据集

![image-20220818190104055](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818190104055.png)

#### 标准结构

![image-20220818191005908](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818191005908.png)

#### Softmax

![image-20220818193109084](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818193109084.png)

### 最后一层，BCE Loss       右边为NLL损失

![image-20220818194208770](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818194208770.png)

![image-20220818195352174](../../AppData/Roaming/Typora/typora-user-images/image-20220818195352174.png)

![image-20220818200333945](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818200333945.png)

- View()函数用于改变张量形状

![image-20220818200710405](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818200710405.png)

自动计算行，784列

![image-20220818201521033](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818201521033.png)

![image-20220818201948326](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818201948326.png)

- momentum用加大下降的幅度，加速模型的收敛

![image-20220818202651862](https://img-1301878935.cos.ap-nanjing.myqcloud.com//typora/image-20220818202651862.png)

- with使得代码可以保证运行完毕后执行某一项操作

- 傅里叶变换可以用于整张图片的特征提取，将时域函数转变为频域表示。典型的有FFT(快速傅里叶变换)，傅里叶变换都是正弦波，对于周期性不是很好的输出，拟合效果不好。更好的方法是小波变换wavelet(函数可以伸缩平移)



