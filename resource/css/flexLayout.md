# flex布局教程(一)
flex是flexible box 的缩写。意思为“**弹性布局**”，是盒子模型的灵活体现。

## **一、Flex容器的属性**
设置在容器本身上面。
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

### **4.justify-content属性**
justify-content属性定义了项目在`主轴(即水平方向)上的对齐方式`。

> justify-content属性有五个值，分别为：`flex-startc | flex-end | center 
| space-between | space-around`。
>
>* flex-start(默认值)：在主轴上，`左边依次对齐`，margin-left值为零。
>* flex-end:在主轴上,`从右边依次对齐`，margin-right为零。
>* center:在主轴上，`居中对齐`，左右两边的距离相等，例如margin:0 auto。
>* space-between:在主轴上，`两端对齐`，项目之间的距离都相等，两端的外边距离都为零。
>* space-around:在主轴上，每个项目`两端的间隔相等`。所以项目之间的间隔比项目与边框的间隔大一倍。

### **5.align-items属性**
align-items属性定义项目如何在`交叉轴对齐`。
> align-items属性有四个值，分别为：`flex-start | flex-end | center | baseline | stretch`。
>* flex-start属性：交叉轴的`起点对齐`。
>* felx-end属性：交叉轴的`结点对齐`。
>* center属性：交叉轴的`中点对齐`。
>* baseline属性：项目的第一行文字的`基线(底线)对齐`。
>* strech(默认值)属性：如果项目没有设置高度或者设置为auto，将占满整个容器的高度。

### **6.align-content属性**
align-content属性定义了`多根轴线的对齐方式`。如果项目只有一条轴线，则该属性不起作用。
> align-content属性有六个值，分别为：`flex-start | flex-end | center | space-between | space-around | stretch` 。
>* flex-start属性：与交叉轴的`起点对齐`。
>* flex-end属性：与交叉轴的`结点对齐`。
>* center属性：与交叉轴的`中点对齐`。
>* space-between属性：与交叉轴的`两端对齐，轴线之间的间隔平均分布`。
>* space-between属性：每根轴线的`两端的间隔相等`，所以，`轴线之间的间隔比轴线与边框的间隔大一倍`。
>* stretch属性：轴线占满整个交叉轴。