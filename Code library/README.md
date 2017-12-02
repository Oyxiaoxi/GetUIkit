# Css Code library

## 1.黑白图像
> 这段代码会让你的彩色照片显示为黑白照片
```css
img.desaturate {
    filter: grayscale(100%);
	-webkit-filter: grayscale(100%);
	-moz-filter: grayscale(100%);
	-ms-filter: grayscale(100%);
    -o-filter: grayscale(100%)
}
```

## 2.页面顶部阴影
> 可以给网页加上漂亮的顶部阴影效果
```css
body:before {
	content: "";
	position: fixed;
	top: -10px;
	left: 0;
	width: 100%;
	height: 10px;

	-webkit-box-shadow: 0 0 10px rgba(0,0,0,.8);
	-moz-box-shadow: 0 0 10px rgba(0,0,0,.8);
	-box-shadow: 0 0 10px rgba(0,0,0,.8);

	z-index: 100
}
```

## 3.所有一切都垂直居中
> 要将所有元素垂直居中
```css
html,body {
	height: 100%;
	margin: 0;
}

body {
	-webkit-align-items: center;
	-ms-flex-align: center;
	align-iterms: center;
	display: -webkit-flex;
	display: flex
}
```

## 4.逗号分隔的列表
```css
ul > li:not(:last-child)::after {
    content: ",";
}
```

## 5.表格单元格等宽
```css
.calendar {
    table-layout: fixed;
}
```

## 6.用 Flexbox 摆脱外边距的各种 hack
```css
.list {
    display: flex;
    justify-content: space-between;
}

.list .person{
    flex-basis: 23%
}
```

## 7.使用属性选择器用于空链接
> 当a元素没有文本值，但 href 属性有链接的时候显示链接：
```css
a[href^="http"]:empty::before {
    content: attr(href);
}
```

## 8.calc() 的使用
> calc() 用法类似于函数，能够给元素设置动态的值
```css
.simpleBlock {
	width: calc(100% - 100px);
}

.complexBlock {
	width: calc(100% - 50% / 3);
	padding: 5px calc(3% - 2px);
	margin-left: calc(10% + 10px)
}
```

## 9.禁用鼠标事件
> CSS3 新增的 pointer-events 让你能够禁用元素的鼠标事件
```css
.disabled {
    pointer-events: none;
}
```

## 10.模糊文本
> 简单但很漂亮的文本模糊效果
```css
.blur {
    color: transparent;
    text-shadow: 0 0 5px rgba(0,0,0,0.5);
}
```