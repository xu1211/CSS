
# tailwind css
absolute	  position: absolute;   绝对定位
relative	  position: relative;   相对定位


right-*       	right: 0px;       absolute定位元素

overflow-hidden	overflow: hidden;   剪辑溢出内容

invisible	      visibility: hidden; 隐藏不可见

## flex 布局
flex	    display: flex;
flex-col	flex-direction: column; 布局方向-垂直
flex-row  flex-direction: row;    布局方向-水平
flex-wrap flex-wrap: wrap;        换行
grow/flex-grow	flex-grow: 1;               扩展填充

### flex中Items 元素间距
gap-*     gap: 0px;           行列
gap-x-*   column-gap: 0px;    列 
gap-y-*   row-gap: 0px;       行

### Items 元素尺寸
w-*       width:
max-w-*   max-width:
min-w-*   min-width:
h-*

### Items 对齐
items-start	    align-items: flex-start;
items-center	  align-items: center;
items-end	      align-items: flex-end;
items-baseline	align-items: baseline;

### Justify 横轴对齐方式
justify-start   justify-content: flex-start;    靠起点
justify-end     justify-content: flex-end;      靠末端
justify-center  justify-content: center;        居中
justify-between justify-content: space-between; 均匀占满
justify-around  justify-content: space-around;  均匀间隔

flex-1	flex: 1 1 0%;

## 间距
### Padding 填充内边距
pt-*        padding-top: 0px;     顶部填充
pb-*        padding-bottom: 0px;  底部填充
pl-*        padding-left: 0px;    左侧填充
pr-*	      padding-right: 0px;   右侧填充
px-*	      padding-left: 0px;  padding-right: 0px;   水平填充
py-*	      padding-top: 0px;   padding-bottom: 0px;  垂直填充
p-*         padding: 0px;   所有侧面的填充

### Margin 元素一侧的边距
mt-*      	margin-top: 0px;
mb-*      	margin-bottom: 0px;
mr-*
mx-*
m-*


## 字体
font-normal     font-weight:
font-semibold

text-xs         字体大小 xs
text-sm
text-base
text-xl

text-right	    text-align: right;
text-center

text-gray-*     灰色
text-blue-*     蓝色

line-through	  text-decoration-line: line-through;   下划线
italic	        font-style: italic;                   斜体
uppercase	      text-transform: uppercase;            大写

break-all	      word-break: break-all;  单词自动换行


## border 边框
border-gray-*	  border-color:灰
border-t        border-top-width: 1px;  边框宽度
border-b	      border-bottom-width: 1px;
border-l        border-left-width: 1px;

## background
bg-white	      background-color: rgb(255 255 255);



## 交互
### 光标
cursor-pointer	cursor: pointer;    指示链接的指针
cursor-wait	    cursor: wait;       程序正忙(转圈)

## 动画
animate-spin	                      转圈
```
animation: spin 1s linear infinite;
@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
```