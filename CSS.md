CSS初学者课程
============
课程视频地址:[为初学者准备的：CSS 速成](https://www.bilibili.com/video/BV1bW411R7hg) <br>
Cascading Stylesheets `层叠样式表`<br>
```html
p{
  color : red;
}
```
三种方式添加CSS
------
1. 外部样式表
  * CSS保存在.css文件中
  * 在HTML里实用<link>引用
2. 内部样式表
  * 不使用外部CSS文件
  * 将CSS放在HTML<style>里
3. 内联样式
  * 仅影响一个元素
  * 在HTML元素的style属性中添加`(不推荐使用)`
  
CSS选择器
----------
1. 

CSS里的颜色
----------
1. 关键词
  * black, silver, white
2. 十六进制
  * #ff0000
3. RGB
  * rgb(255, 0, 0)
4. HSL
  * hsl(0, 100%, 50%) (hue色相, saturation饱和度, lightness明度)
  ![](https://pic3.zhimg.com/v2-62391ef2080831c1941e3170997fac8a_r.jpg)  
5. RGBA
  * rgb(255, 0, 0, 0.5)
6. HSLA

盒子模型
---------
margin外边距->border边框->padding内边距->`content`
外边距重叠:大边吃小边<br>
指定段落块间距离:
```html
p{
  marigin-top : 5px;
  marigin-bottom : 5px;
  marigin-right : 10px;
  marigin-left : 10px;
}
p{
  marigin: 5px 10px 5px 10px;
}
p{
  margin: 5px 10px; 
}
<!----第一个值代表上下,第二个代表左右--->
```
此处也可以改成内边距paddding/指定顺序为上右下左(顺时针)

CSS中的定位方法
----------
static-静态定位
relative-相对定位
absolute-绝对定位
fixed-固定定位
sticky
