[TOC]



# 1.html学习







# 2.css学习

目标:

> 1. 学会使用CSS选择器
> 2. 熟记CSS样式和外观属性
> 3. 熟练掌握CSS各种选择器
> 4. 熟练掌握CSS各种选择器
> 5. 熟练掌握CSS三种显示模式
> 6. 熟练掌握CSS背景属性
> 7. 熟练掌握CSS三大特性
> 8. 熟练掌握CSS盒子模型
> 9. 熟练掌握CSS浮动
> 10. 熟练掌握CSS定位
> 11. 熟练掌握CSS高级技巧强化CSS





## css盒子模型





## 浮动float





## 定位position

### 1.边偏移

包括top，left，bottom，right。

### 2.定位模式

1. 静态定位static（不多讲标准流不可边偏移）
2. 相对定位relative（自恋型-相对于自己（左上角）移动，脱标但站位置）
3. 绝对定位absolute（<u>相对与有定位的父盒子偏移</u>，无父时相对与浏览器偏移，完全脱标不占据位置）
4. 固定定位fixed（悟空型，不管有无父盒子只认浏览器窗口，完全脱标不占位置）

### 3.子绝父相

eg：.father｛ position：relative；top：10px； left：20px；｝

​        .son｛position:absolution;｝-------------------------------------------**子绝父相**相当于浮动里面的清除浮动，因为父盒子relative是站位置的。



## css高级特性

### 1.显示与隐藏（display与visibility区别）

a

display：none；隐藏不占位置

display：block；显示

b

visibility：hidden；隐藏占位置

visibility：visible；显示

### 2.overflow（溢出）

属性值：

visible显示

hidden隐藏

scroll总是显示滚动条

auto溢出时显示滚动条

### 3.鼠标样式

cursor: default;/*鼠标小白*/
cursor: text;/*文本*/
cursor:pointer;/*小手*/*/
cursor:move;/*拖拽*/

### 4.outline轮廓线

运用于input输入框，textarea等外面默认的蓝色边框（不是边框）

outline：none；取消轮廓线

eg

<input type="text" name="" id="" value="" />

input {
			outline: none;
			border: 1px solid red;
		    }

### 5.textarea取消拖拽

resize:none;

eg

<textarea name="" rows="" cols=""></textarea>

textarea {
		    	resize:none;
		    }

### 6.vertical-align垂直对齐

文字分为行高----包括顶线，中线，基线，底线

eg

		<div>
			<img src="img/tudou.jpg"/>
			<e>我是文字jsgf</e>
		</div>
	css		img {
				vertical-align:middle;图片相对与文字中线对齐
				vertical-align: top;
				vertical-align: baseline;
				/*vertical-align: bottom;*/
			}
			div {
				border:2px solid red;
			}