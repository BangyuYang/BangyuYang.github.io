# flex布局教程(二)
flex是flexible box 的缩写。意思为“**弹性布局**”，是盒子模型的灵活体现。

## **flex项目的属性**
>1. order
>2. flex-grow
>3. flex-shrink
>4. flex-basis
>5. flex
>6. align-self

### **1.order属性**
order属性定义项目的排列顺序。数值越小，排列越靠前。默认值为0.

>* order属性在item只有数字：integer。

### **2.flex-grow**
flex-grow属性定义项目的`放大比例`，默认为0，即使存在剩余空间，也不放大。

>* felx-grow；number,默认为0。
> 
> 如果所有项目的flex-grow值都为1，则他们等分空间(存在的话)，如果一个项目的flex-grow值为2，其他的都为1的话，则值为2的占据的剩余空间比1大。

### **3.flex-shrink属性**

flex-shrink属性定义了项目的`缩小比例`，默认值为1，即空间不足的话，该项目将会缩小。
>* flex-shrink：number,默认值为1。
>
> 如果所有项目的flex-shrink属性都为1，当空间不足的话，都将等比例缩小。如果一个项目的flex-shrink为0，其他的都为1的话，当空间不足时，值小的不缩小。负值对该属性无效。

### **4.flex-basis**
flex-basis属性定义了分配多余空间之前，项目占据主轴空间(mian size)。浏览器根据这个属性计算主轴书否有多余的空间。它的默认值为auto，即项目的本来大小。
>* flex-basis: length | auto,默认值为auto。
>
> 它可以设置固定的值(例如100px),项目就会占据固定的空间。

### **5.flex属性**
flex属性是flex-grow,flex-shrink,flex-basis的简写，默认值为1 0 auto。后两个属性为可选。
>* flex: none | [ `flex-grow` `flex-shrink` ? || `flex-basis` ]
>
> 该属性有两个快捷值：auto(1 1 auto)h和 none(0 0 auto)。
>
> `建议优先使用这个属性，而不是单独分开写三个属性，因为浏览器会推算相关值`。

### **6.align-self**
align-self属性`允许单个项目和其他项目有不一样的对齐方式`，可覆盖align-items属性。默认值为auto，表示继承父元素align-items属性，如果没有父元素，则继承stretch。
>* align-self: auto | flex-start | flex-end | center | baselline | stretch。
>
>该属性也可能取6个值，除了auto，其他的都跟align-items一样。


