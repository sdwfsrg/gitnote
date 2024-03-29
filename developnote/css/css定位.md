# css定位

## 定位和浮动

定位的基本思想  它允许你定义的元素框相对于其正常位置应该出现的位置，货值相对于父元素、另一个元素设置浏览器窗口本身的位置   

### 相对定位
```
#box_relative {
  position: relative;
  left: 30px;
  top: 20px;
}
```

![相对定位](http://www.w3school.com.cn/i/ct_css_positioning_relative_example.gif)

在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其他框

### 绝对定位
设置为绝对定位的元素框从文档流完全删除，并相对于其包含块定位，包含块可能是文档中的另一个元素或者是初始包含块。元素原先在正常文档流中所占的空间会关闭，就好像该元素原来不存在一样。元素定位后生成一个块级框，而不论原来它在正常流中生成何种类型的框。
```
#box_relative {
  position: absolute;
  left: 30px;
  top: 20px;
}
```
![绝对定位](http://www.w3school.com.cn/i/ct_css_positioning_absolute_example.gif)

绝对定位的元素的位置相对于最近的已定位的祖先元素，如果元素没有已定位的祖先元素，那么它的位置相对于最初的包含块（画布或者HTML元素）
因为绝对定位的框和文档流无关，所有他们可以覆盖页面上的其他元素，可以通过设置z-inde属性来控制这些框的堆放次序

浮动的框可以向左或者向右移动，直到它的外边缘碰到包含框或另一个浮动框的边框为止。 由于浮动框不在文档的普通流中，所以文档的普通流中块框表现的就像浮动框不存在一样

![浮动](http://www.w3school.com.cn/i/ct_css_positioning_floating_right_example.gif)


![](http://www.w3school.com.cn/i/ct_css_positioning_floating_left_example.gif)

![](http://www.w3school.com.cn/i/ct_css_positioning_floating_left_example_2.gif)
css中**float** 属性实现元素浮动 （left，right ，none，inherit）
clear：both；在左右两侧均不允许浮动元素。


