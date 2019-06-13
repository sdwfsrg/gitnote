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

###

在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其他框

浮动的框可以向左或者向右移动，直到它的外边缘碰到包含框或另一个付东凯的边框为止。 由于浮动框不在文档的普通流中，所以文档的普通流中块框表现的就像浮动框不存在一样
css中**float** 属性实现元素浮动 （left，right ，none，inherit）
clear：both；在左右两侧均不允许浮动元素。


