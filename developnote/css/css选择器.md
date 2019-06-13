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
