# css样式

## 背景
background-color：;
background-image：url（‘bgimg.png’）;
background-position:center;(50% 50%  50px 50px)
background-repeat:repeat-y;
background-attachment: fixed;防止滚动，声明相对于可视区是固定的



属性	描述
background	简写属性，作用是将背景属性设置在一个声明中。
background-attachment	背景图像是否固定或者随着页面的其余部分滚动。
background-color	设置元素的背景颜色。
background-image	把图像设置为背景。
background-position	设置背景图像的起始位置。
background-repeat	设置背景图像是否及如何重复。
## 文本
属性 | 描述
:-------:|:---:
color	|设置文本颜色
direction	|设置文本方向。
line-height	|设置行高。
letter-spacing	|设置字符间距。
text-align	|对齐元素中的文本。
text-decoration	|向文本添加修饰。
text-indent	|缩进元素中文本的首行。
text-shadow	|设置文本阴影。CSS2 包含该属性，但是 CSS2.1 没有保留该属性。
text-transform	|控制元素中的字母。
unicode-bidi	|设置文本方向。
white-space	|设置元素中空白的处理方式。
word-spacing	|设置字间距。
## 字体
属性| 描述
:---:|:---:
font	|简写属性。作用是把所有针对字体的属性设置在一个声明中。
font-family	|设置字体系列。
font-size	|设置字体的尺寸。
font-size-adjust	|当首选字体不可用时，对替换字体进行智能缩放。（CSS2.1 已删除该属性。）
font-stretch	|对字体进行水平拉伸。（CSS2.1 已删除该属性。）
font-style	|设置字体风格。
font-variant	|以小型大写字体或者正常字体显示文本。
font-weight	|设置字体的粗细。

## 链接
## 列表
## 表格

属性	|描述
:--:|:--:
border-collapse	|设置是否把表格边框合并为单一的边框。**separate**	默认值。边框会被分开。不会忽略 border-spacing 和 empty-cells 属性。  **collapse**	如果可能，边框会合并为一个单一的边框。会忽略 border-spacing 和 empty-cells 属性。
border-spacing	|设置分隔单元格边框的距离。  border-spacing:10px 50px;
caption-side	|设置表格标题的位置。top	默认值。把表格标题定位在表格之上。bottom	把表格标题定位在表格之下。
empty-cells	|设置是否显示表格中的空单元格。hide	不在空单元格周围绘制边框。show	在空单元格周围绘制边框。默认 inherit	规定应该从父元素继承 empty-cells 属性的值。
table-layout	|设置显示单元、行和列的算法。automatic	默认。列宽度由单元格内容设定。fixed	列宽由表格宽度和列宽度设定。inherit	规定应该从父元素继承 table-layout 属性的值。
## 轮廓

# css框模型

## 内边距
## 边框
border-style 默认none  想边框必须声明样式
```
p {border-style: solid; border-width: 5px;}

p {
border-style: solid; 
border-width: 15px 5px 15px 5px;
}
p {
  border-style: solid;
  border-top-width: 15px;
  border-right-width: 5px;
  border-bottom-width: 15px;
  border-left-width: 5px;
 border-color: blue red;
  }
上下是蓝左右是红
```
## 外边距
## 外边距合并
外边距合并指的是，当两个垂直外边距相遇时，它们将形成一个外边距。合并后的外边距的高度等于两个发生合并的外边距的高度中的较大者。

当一个元素出现在另一个元素上面时，第一个元素的下外边距与第二个元素的上外边距会发生合并
![](http://www.w3school.com.cn/i/ct_css_margin_collapsing_example_1.gif)

当一个元素包含在另一个元素中时（假设没有内边距或边框把外边距分隔开），它们的上和/或下外边距也会发生合并。
![](http://www.w3school.com.cn/i/ct_css_margin_collapsing_example_2.gif)


假设有一个空元素，它有外边距，但是没有边框或填充。在这种情况下，上外边距与下外边距就碰到了一起，它们会发生合并：

![](http://www.w3school.com.cn/i/ct_css_margin_collapsing_example_3.gif)

如果这个外边距遇到另一个元素的外边距，它还会发生合并

![](http://www.w3school.com.cn/i/ct_css_margin_collapsing_example_4.gif)


![](http://www.w3school.com.cn/i/ct_css_margin_collapsing.gif)
