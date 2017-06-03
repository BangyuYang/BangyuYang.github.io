# flex布局教程(一)
flex是flexible box 的缩写。意思为“**弹性布局**”，是盒子模型的灵活体现。

## **一、Flex的属性**
>1. flex-direction
>2. flex-wrap
>3. flex-flow
>4. justify-conent(个人最常用)
>5. align-items
>6. align-conent

### **1、flex-direction属性**

flex-direction属性决定主轴的方向(即项目的排序方向)他们可以放在两个方向，即水平方向和垂直 方向。

>`flex-direction`的值有四个：**row | row-reverse | column| column-reverse** 
>
>* row(默认值)：主轴为水平方向,项目排序方向`从左至右`堆叠成一行。
>* row-reverse:主轴为水平方向，项目排序方向`从右至左`堆叠成一行。
>* column:主轴为垂直方向,排序方向`从上到下`堆叠成一列。
>* column-reverse:主轴方向为垂直方向，项目排序方向`从下往上`堆叠成一列。

### **2.flex-wrap属性**
flex-warp属性:一般情况下，项目都是排在一条线(也称做主轴)上。如果一条线放不下，就要考虑如何换行，flex-wrap属性提供了三个值。

>flex-wrap三个值分别为：**nowrap | wrap | wrap-reverse;**
>
>* nowrap(默认值):`不换行`，从左至右依次顺序排列。
>* wrap:`换行，第一行在上面`，从左至右依次顺序排列。
>* wrap-reverse: `换行，第一行在下面。`从下面开始一招顺序排列。

### **3.flex-flow属性**
flex-flow属性(适用于parent flex容器元素)是`flex-direction属性`和`flex-wrap属性`的简写形式,默认值为**row nowrap**。