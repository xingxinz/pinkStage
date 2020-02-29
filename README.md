# 使用css3实现导航页切换过渡动画

## 涉及知识
- transition和animation的使用
- transform属性的用法
- font-face自设字体库
- 响应式布局 @media
- boder 绘制简单三角形

## 实现效果：
- 点击底部导航栏可以平滑切换到不同的页面
- 显示适配不同尺寸屏幕

## 实现时具体问题总结
+ 实现过渡与动画  

  * transition需要事件触发，animation不用，一上来就可以加载  
    【分析】  
    （点击导航栏，切换页面，并且页面中的上下段落有碰撞动画）  
    这里切换页面是根据点击触发的，使用transition;  
    碰撞动画直接加载，使用animation.  
  * 使用transform中的translate调整页面的位置变化 
  * 使用：checked匹配每个已被选中的 input 元素

+ 选择器   

  * element>element 只能选择作为某一元素子元素的元素   
  * element+element 相邻兄弟选择器   
  * element~element 后续兄弟选择器   
  * [attribute] 选择带有attribute 属性所有元素。   

- 有些图标可以通过自设字体库实现，页面可以减少加载图片

+ border绘制三角形
  + 内容为空  width:0;height:0
  + 增大border宽度
  + 设置其他边为透明色 transparent
