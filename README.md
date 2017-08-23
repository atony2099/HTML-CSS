# HTML-CSS
hello  html



### 清除浮动 

```
clear:both
```



> 浮动布局之后无法子元素无法撑开父元素，---消除浮动

[CSS clear both清除浮动](http://www.divcss5.com/rumen/r424.shtml)



## 进阶的属性

对多余内容的处理: 

*overfolow:*对超过限定区域内容的处理：滚动or隐藏

*textoverfolow*:针对overflow折叠的情况，进一步美化

> 配合：
>
> > overflow: hidden;  
> >
> > white-space: nowrap;

*whiteSpace*

> how to handle the space
>
> normal  : 1. Sequences of whitespace are collapsed; 2. Lines are broken as necessary to fill line boxes.
>
> nowarap:  suppresses line breaks 







#### 布局系列: 

### position 布局

文档流: 

> 块元素做上到下，
>
> 内联元素做从到右

```css
postion:relative // 相对于 原来位置 移动，不改变文档流
postion:absoulte // 相对于最近的一个父元素的一个relatvie元素，脱离文档流，父元素会坍塌
postion:fixed //相对于浏览器窗口
```

[十步图解CSS的position](http://blog.jobbole.com/49320/#article-comment)

[http://www.cnblogs.com/wangfupeng1988/p/4322680.html](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)

[[css知多少（11）——position](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)



### float布局

> 排序规则:1. 如果上一个元素不是浮动，那垂直位置不变
>
> 2. 如果上一个是浮动的，跟谁后面

**清楚浮动**: 消除浮动的影响，理解为按照文档流布局.消除浮动五大小的问题

[CSS清除浮动_清除float浮动](http://www.divcss5.com/jiqiao/j406.shtml)](http://www.divcss5.com/jiqiao/j406.shtml)











