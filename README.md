[toc]
# CSS


## 定位机制
CSS的定位机制有3种：
1. 文档流
1. 浮动（float：left/right/none）
1. 定位 （position:static/relative/absolute/）。

> 文档流：将窗体自上而下分成一行一行,并在每行中按从左至右的挨次排放元素,即为文档流。\
每个块级元素都独有一行,一切元素均可生成子行用于摆放子元素 浮动元素则按规则浮在行的一端. 若当时行容不下, 则另起新行再浮动。\
有三种状况将使得元素离开文档流而存在,分别是`浮动、绝对定位、固定定位`.


### [float 浮动](./demo/float.html)
  - float：left/right/none;
浮动元素脱离文档流 不占任何文档流空间，
而浮动元素之间的定位照样基于正常的文档流，然后从文档流中抽出并尽能够远的挪动至左侧或许右侧。当一个元素脱离正常文档流后，依然在文档流中的其他元素将忽略该元素并填补其原先的空间。 
float在绝对定位和display为none时不会被应用

### [position 定位](./demo/position.html)
  - position: static;      静态定位,`保持文档流`
  - position: fixed;       固定定位,相对于浏览器固定 `脱离文档流`
  - position: relative;    相对定位,元素相对其正常位置移动 `保持文档流`
  - position: absolute;    绝对定位,元素相对于最近的已定位父元素移动，如果元素没有已定位的父元素，那么它的位置相对于\<html>: `脱离文档流`
  - position: sticky;      粘性定位,元素是依赖于用户的滚动 在 relative 与 fixed 定位之间切换。2017年浏览器才支持

### [display属性](./demo/display.html)
在 css 中实现页面布局的主要方法是设定display属性的值。
每个元素都有该属性,来确定元素类型
  -  none	隐藏元素,不占空间
  -  inline  默认属性内联元素,没宽高属性,不独占一行 (span,输入框,图片,引用...)
  -  block   块级元素,有宽高属性,独占一行 (div,标题,表格,段落....)
  -  inline-block	行内块元素,有宽高属性又不独占一行
  -  table   块级表格
  -  flex    弹性盒

### [溢出元素处理](./demo/overflow.html)
  - overflow: visible;
    - visible	默认值。内容不会被修剪，会呈现在元素框之外。
    - hidden	内容会被修剪，并且其余内容是不可见的。
    - scroll	内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。
    - auto	    如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。
    - inherit	规定应该从父元素继承 overflow 属性的值。

## css layout 网页布局
https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout
- 流布局
默认的 HTML 文档流 布局
- 浮动 + 定位
布局的传统解决方案，基于盒状模型，依赖 display 属性 + position 属性 + float 属性。
- Flex box 弹性布局
`display:flex`
设计横向或纵向的布局

http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html

任何一个容器都可以指定为 Flex 布局。设为 Flex 布局以后子元素的float、clear和vertical-align属性将失效。

采用 Flex 布局的元素，称为 Flex 容器（flex container），简称"容器"。它的所有子元素自动成为容器成员



- grid 网格布局
`display: grid`
设计用于同时在两个维度上把元素按行和列排列整齐(像二维网格一样)。

- 表格布局