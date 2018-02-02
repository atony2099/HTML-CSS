# 是什么？
指定行内元素垂直对齐方式
[vertical](https://developer.mozilla.org/zh-CN/docs/Web/CSS/vertical-align)

/* keyword values */
vertical-align: baseline;
vertical-align: sub;
vertical-align: super;
vertical-align: text-top;
vertical-align: text-bottom;
vertical-align: middle;
vertical-align: top;
vertical-align: bottom;

相对一般是父元素==


## 解决图片不充分问题
默认情况下 vertical-align: baseline;
导致图片会对齐父元素中的基线(父元素的基线也就是它内部的文本的基线)，由于基线到父容器的底部还有一段距离，导致底部有空白
