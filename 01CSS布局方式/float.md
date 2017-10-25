[All About Floats](https://css-tricks.com/all-about-floats/)

需要解决的问题：
1. float 对其他元素的影响
2. 如何清除浮动

### float
文档流：从上到下，从做到右
脱离了正常的文档流
<!-- 排版方式,让元素浮动起来，其他元素把他环绕起来，**remain a part of the flow of the web page** -->
float:left right  none

#### 元素对紧跟着的非浮动元素的影响:
- 块状元素浮动的影响:其他块状元素会上浮，顶替他的位置 对内联元素的影响:其他内联元素会紧挨着他
- 内联元素浮动的影响：其他块状元素会上浮，顶替他的位置， 对内联元素和的影响：其他内联元素会紧挨着他

#### float元素的排版规则
高度都相等:  容不下换行.
高度不相等的时候:容不下换行


#### clean float
浮动

> 浮动布局的问题:高度坍塌
