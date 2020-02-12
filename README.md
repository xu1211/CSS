# CSS
 css布局

## 常用属性
CSS的定位机制有3种：文档流、浮动（float：left/right/none）和定位 （position:static/relative/absolute/）。

> 文档流：将窗体自上而下分成一行一行,并在每行中按从左至右的挨次排放元素,即为文档流。\
每个块级元素都独有一行,一切元素均可生成子行用于摆放子元素 浮动元素则按规则浮在行的一端. 若当时行容不下, 则另起新行再浮动。\
有三种状况将使得元素离开文档流而存在,分别是`浮动、绝对定位、固定定位`.


### display
每个元素都有该属性,来确定元素类型
  -  none	隐藏元素,不占空间
  -  inline  默认属性内联元素,没宽高属性,不独占一行 (span,输入框,图片,引用...)
  -  block   块级元素,有宽高属性,独占一行 (div,标题,表格,段落....)
  -  inline-block	行内块元素,有宽高属性又不独占一行
  -  table   块级表格
  -  flex    弹性盒



### 浮动
    - float：left/right/none;
浮动元素脱离文档流 不占任何文档流空间，
而浮动元素之间的定位照样基于正常的文档流，然后从文档流中抽出并尽能够远的挪动至左侧或许右侧。当一个元素脱离正常文档流后，依然在文档流中的其他元素将忽略该元素并填补其原先的空间。 

### position 定位
    - position: static;      静态定位,保持文档流
    - position:fixed;        固定定位,相对于浏览器固定 脱离文档流
    - position:relative;     相对定位,元素相对其正常位置移动 保持文档流
    - position:absolute;     绝对定位,元素相对于最近的已定位父元素移动 脱离文档流
    - position: sticky;      粘性定位,元素是依赖于用户的滚动 在 relative 与 fixed 定位之间切换。



### 溢出元素处理
    - overflow: visible;
        - visible	默认值。内容不会被修剪，会呈现在元素框之外。
        - hidden	内容会被修剪，并且其余内容是不可见的。
        - scroll	内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。
        - auto	    如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。
        - inherit	规定应该从父元素继承 overflow 属性的值。
