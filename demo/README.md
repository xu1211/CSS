# css flex布局
弹性盒子模型

Flex容器（flex container）所有子元素自动成为容器成员，称为Flex项目（flex item）
![alt 属性文本](./flex/flex.png)

ref: https://www.runoob.com/w3cnote/flex-grammar.html

## [flex](./flex/flex.html) 布局
display: flex;

### [flex direction](./flex/flex-direction.html) 布局方向
flex-direction: row 水平|row-reverse 水平逆向|column 垂直|column-reverse 垂直逆向|initial 默认|inherit 继承父;

### [flex align](./flex/flex-align.html) 对齐方式
align-items: stretch|center|flex-start|flex-end|baseline|initial|inherit;

### flex grow\shrink\basis 子元素空间
flex: 扩展量flex-grow 收缩量flex-shrink 长度flex-basis|auto|initial|inherit;

### flex wrap 弹性换行
flex-wrap: wrap;


// 间距
gap: 0px;
column-gap: 0px;
row-gap: 0px;

// dimension 尺寸 高度和宽度
height:100px;
width:100px;
min-width: 0px;
max-width: 0px;



// 文字粗细
font-weight: 600; 



place-items: center;
justify-items: center;
```
