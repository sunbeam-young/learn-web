# 1. BFC
  * ## 定义：
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BFC(Block formatting context)直译为"块级格式化上下文"。它是一个独立的渲染区域，只有Block-level box参与， 它规定了内部的Block-level Box如何布局，并且与这个区域外部毫不相干。

  * ## 布局规则：
    - 内部的Box会在垂直方向，一个接一个地放置。
    - Box垂直方向的距离由margin决定。属于同一个BFC的两个相邻Box的margin会发生重叠。
    - 每个元素的margin box的左边， 与包含块border box的左边相接触(对于从左往右的格式化，否则相反)。即使存在浮动也是如此。
    - BFC的区域不会与float box重叠。
    - BFC就是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素。反之也如此。
    - 计算BFC的高度时，浮动元素也参与计算
    
  * 参考链接：
    - http://www.cnblogs.com/lhb25/p/inside-block-formatting-ontext.html
    - https://segmentfault.com/a/1190000012221820