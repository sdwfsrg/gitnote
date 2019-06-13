## 选择器
### 派生选择器
**根据元素在其位置的上下文关系来定义样式**

*如果希望列表中 的strong变斜体*
```
li strong {
  font-style:italic;
  font-weight:normal;
}


<p><strong>我是粗体字，不是斜体字，因为我不在列表当中，所以这个规则对我不起作用</strong></p>

<ol>
<li><strong>我是斜体字。这是因为 strong 元素位于 li 元素内。</strong></li>
<li>我是正常的字体。</li>
</ol>
```

##  id选择器

##  类选择器

## 属性选择器



## 元素选择器

## 类型选择器

## 通配符选择器
   （*） 代表所有元素

## 选择器分组

## 后代选择器（包含选择器）
```
h1 em {color:red;}
```
作为 h1 元素后代的任何 em 元素   或者
包含 em 的所有 h1 会把以下样式应用到该 em
(子或者孙或者孙孙孙)

## 子元素选择器
（和后代选择器的区别 指定元素只有子元素）
## 相邻兄弟选择器

增加紧接在 h1 元素后出现的段落的上边距
```
h1 + p {
margin-top:50px;
}
```
选择紧接在 h1 元素后出现的段落，h1 和 p 元素拥有共同的父元素

```
<div>
  <ul>
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
  </ul>
  <ol>
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
  </ol>
</div>
```






