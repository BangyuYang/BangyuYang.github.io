# css布局篇(一)之Flex布局
flex是flexible box 的缩写。意思为“弹性布局”，是盒子模型的灵活体现。

## 一、Flex的属性
>* flex-direction
>* flex-wrap
>* flex-flow
>* justify-conent(个人最常用)
>* align-items
>* align-conent

### 1、flex-direction属性

flex-direction属性决定主轴的方向(即项目的排序方向)。

>flex-direction的值有四个：row | row-reverse | column | column-reverse 
>* row(默认值)：主轴为水平方向,项目排序方向从左至右。
>* row:主轴为水平方向，项目排序方向从右至左。
>* column:主轴为垂直方向,排序方向从上到下。
>* column-reverse:主轴方向为垂直方向，项目排序方向从下往上。