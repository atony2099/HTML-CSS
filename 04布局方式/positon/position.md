

# html 的 positon

## static
默认的

## absolute
是否保留文档流位置:否，文档流里根本没有他的位置
相对的元素：第一个非static元素


## relateive
是否保留文档流位置： 是，保留文档的位置，只是视觉上他发生了偏移
相对元素：自己
应用场景： 作为absolute的包含快

## fixed
相对元素： 浏览器窗口

#reactNative 的postion
所有元素默认都是relative;

> position in React Native is similar to regular CSS, but everything is set to relative by default, so absolute positioning is always just relative to the parent

## postion 实战
1. 设置居中
```
child {
    position: absolute;
    top: 50%;  /* position the top  edge of the element at the middle of the parent */
    left: 50%; /* position the left edge of the element at the middle of the parent */

    transform: translate(-50%, -50%); /* This is a shorthand of
                                         translateX(-50%) and translateY(-50%) */
}
```
![]()
