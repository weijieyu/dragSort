# DragSort

拖拽排序小组件

[demo在线演示地址](http://yujieyu7.github.io/drag/)

使用方法，在页面引入 dragSort.js 文件，添加如下代码

var dragLi = new Drag() //创建拖拽对象

dragLi.init((obj,towards,opt) //初始化调用
/*
配置参数，依次为

1.obj 被拖拽的元素，传入任意一个就可以

2.towards 碰撞检测时的检测条件，值为width/height 代表水平和垂直方向，默认为height

3.回调函数，json格式，依次为目标元素mousedown，mousemove,mouseup是所执行的，默认为空函数
{
	'cbDown': function(){},
	'cbMove': function(){},
	'cbUp': function(){}
}

/*

dragLi.addDrag()//给他的兄弟也添加上拖拽
