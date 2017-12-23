# FLex布局

[理解Flexbox：你需要知道的一切](https://www.w3cplus.com/css3/understanding-flexbox-everything-you-need-to-know.html)

[Flex布局完全指南](https://zhuanlan.zhihu.com/p/25984121)

[Flex 布局教程：语法篇
](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)

## 总览

![](http://ohbzayk4i.bkt.clouddn.com/17-12-4/6932375.jpg)
![](http://ohbzayk4i.bkt.clouddn.com/17-12-4/92488922.jpg)
![](http://ohbzayk4i.bkt.clouddn.com/17-12-4/46247106.jpg)
![](http://ohbzayk4i.bkt.clouddn.com/17-12-4/49394493.jpg)
![](http://ohbzayk4i.bkt.clouddn.com/17-12-4/22941756.jpg)









## flex容器

![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071004.png)

## flex-direction
在主轴上的排列方式
![](http://ohbzayk4i.bkt.clouddn.com/17-12-2/78662264.jpg)

## flex-wrap
换行方式

- no warp(不换行，默认)
![](http://ohbzayk4i.bkt.clouddn.com/17-12-2/56809936.jpg)

- warp
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071008.jpg)

- wrap-revesed
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071009.jpg)


## justify-content
在主轴对齐方式
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071010.png)


##  align-items
在主轴上的对齐方式
![](https://pic3.zhimg.com/50/v2-7b84a2730c8037555857cb44de2f7346_hd.jpg)
- flex-start: 按照交叉轴的起点对齐。
- flex-end: 按照交叉轴的终点对齐。
- center: 沿交叉轴方向居中。
- baseline: 按照项目的第一行文字的基线对齐。
- stretch: 默认值，在满足子项目所设置的min-height、max-height、height的情况下拉伸子元素使之填充整个父元素。


## align-content属性
多行元素的时候 排列方式
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071012.png)



# Item 属性
在主轴上


## order 排序
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071013.png)

## flex-grow flex-shrink
存在剩余空间瓜分剩余空间的比率
(默认是0，不瓜分剩余空间)

如果所有项目的flex-grow属性都为1，则它们将等分剩余空间（如果有的话）。如果一个项目的flex-grow属性为2，其他项目都为1，则前者占据的剩余空间将比其他项多一倍。

![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071014.png)

flex-shrink:
空间不足时候缩小的比率
> flex-shrink默认值为1， 当所有子元素都为默认值时，则空间不足时子元素会同比例缩小。如果其中某个子元素的flex-shrink值为0，则空间不足时该子元素并不会缩小。如果其中某个子元素的flex-shrink值为2时，则空间不足时该子元素会以二倍速度缩小。
![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071015.jpg)


## flex-basis

item的宽度，默认宽度是 auto(自适应内容)


## align-self
单个项目 ，覆盖align-items

![](http://www.ruanyifeng.com/blogimg/asset/2015/bg2015071016.png)


## flex
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}

```
flex:auto  = flex: 1 1 auto
flex:none = flex :0,0, auto

```
