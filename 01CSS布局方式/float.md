[All About Floats](https://css-tricks.com/all-about-floats/)
[CSS float 浮动属性](http://www.cnblogs.com/polk6/archive/2013/07/25/3142187.html)
[What does the CSS rule “clear: both” do?](https://stackoverflow.com/questions/12871710/what-does-the-css-rule-clear-both-do)
[在线code](https://codepen.io/anon/pen/BwggMW)

需要解决的问题：
1. float 对其他元素的影响
2. 如何清除浮动


> The float CSS property specifies that an element should be placed along the left or right side of its container,  **allowing text and inline elements to wrap around it**



### float
文档流：从上到下，从做到右
脱离了正常的文档流，但是还是保留了位置，从而得以让文字和内联元素 包裹它
<!-- 排版方式,让元素浮动起来，其他元素把他环绕起来，**remain a part of the flow of the web page** -->
float:left right  none

#### 元素对紧跟着的非浮动元素的影响:
- 块状元素浮动的影响:其他块状元素会上浮，顶替他的位置，**但是内容区域是从float元素开始计算的** 对内联元素的影响:其他内联元素会紧挨着他
- 内联元素浮动的影响：其他块状元素会上浮，顶替他的位置， 对内联元素和的影响：其他内联元素会紧挨着他

#### float元素的排版规则
高度都相等:  容不下换行.
高度不相等的时候:容不下换行


#### 清除浮动
为什么需要清除浮动
1. 由于float的元素不在文档流中，相邻的块状元素会顶上去，使用clear消除后像之前那样正常布局
2. 对父类元素的影响，清除后父元素的高度被撑起来了
清除浮动的作用：清除后元素的高度被撑起来了
> 想象float元素在被clear之前是不知道高度的


> 浮动布局的问题:高度坍塌
