
# BLOCK, inline, inline-block
[block，inline和inline-block概念和区别](http://www.cnblogs.com/KeithWang/p/3139517.html)

- block : 独占一行；盒子属性都有效
   常见的有: Div,H1~H6, P, UL
- inline: 挤在一起，只能设置左右左右的margin 和 padding;常见的规律:inline只能包含inline
   常见的有: span,img,a

- inline-block： 跟别人挤在一起，但是可以像block那样设置盒子:input


# float布局
[CSS float浮动的深入研究、详解及拓展(一)](http://www.zhangxinxu.com/wordpress/2010/01/css-float%E6%B5%AE%E5%8A%A8%E7%9A%84%E6%B7%B1%E5%85%A5%E7%A0%94%E7%A9%B6%E3%80%81%E8%AF%A6%E8%A7%A3%E5%8F%8A%E6%8B%93%E5%B1%95%E4%B8%80/)理解float:相当于有方向的 inline-block;最初是为了解决文字环绕的问题
高度欺骗: 欺骗父元素让他误以为他们有高度，从而导致父元素的坍塌
**实际还是处在文档流中的**
> 排序规则:1. 如果上一个元素不是浮动，那垂直位置不变
>
> 2. 如果上一个是浮动的，跟谁后面

**清楚浮动**: 消除浮动的影响，理解为按照文档流布局.消除浮动五大小的问题

[CSS清除浮动_清除float浮动](http://www.divcss5.com/jiqiao/j406.shtml)](http://www.divcss5.com/jiqiao/j406.shtml)

> 深入理解:浮动具有破坏性，她欺骗了父元素，让父元素觉得他的inline-height= 0;  无法撑起高度，但是他的高度和宽度实实在在在那边，其他元素穿不过去T它


# position 布局

```css
- 包含absolute,  fixted, relateive, static
- 常用absoulte, 针对第一个非static 定位
postion:relative // 相对于 原来位置 移动，不改变文档流
postion:absoulte // 相对于最近的一个父元素的一个非static元素，
postion:fixed //相对于浏览器窗口
```

- 脱离文档流，浮动在上面


[十步图解CSS的position](http://blog.jobbole.com/49320/#article-comment)

[http://www.cnblogs.com/wangfupeng1988/p/4322680.html](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)

[[css知多少（11）——position](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)](http://www.cnblogs.com/wangfupeng1988/p/4322680.html)



# 伪类 伪元素

> 都是虚伪的:  没有在dom节点中
> Â
> ![](http://ohbzayk4i.bkt.clouddn.com/17-8-26/50543438.jpg)









# 进阶的属性

**min_height**，**max_height**：盒子最小和最大高度







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
