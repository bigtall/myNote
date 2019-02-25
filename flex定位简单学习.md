## flex定位

* 用法：

.box{
    display:flex;
    display: -webkit-flex; /* Safari webit内核的浏览器 */
  }

* 常用的几个点
* 1、 flex-direction属性决定主轴的方向（即项目的排列方向）。
      row 默认值 水平方向，起点在左（从左往右）
      row-reverse 水平方向 起点在右（从右往左）
      column 垂直方向 从上往下
      column-reverse 垂直方向 从下玩上


* 2、 justify-content属性定义了项目在主轴上的对齐方式。

justify-content: flex-start | flex-end | center | space-between | space-around;

* 3、 align-items属性定义项目在交叉轴上如何对齐。

align-items: flex-start | flex-end | center | baseline | stretch;

* 综上：实现水平垂直居中，将父级元素进行flex定位;

.body{
   display: flex;
   display: -webkit-flex;
   justify-content:space-between;
   align-items: stretch;
   flex-wrap: wrap;
}






