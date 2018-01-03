## CSS盒模型详解
> 每个html标签都是一个方块，然后这个方块又包着几个小方块，如同盒子一层层的包裹着，这就是所谓的盒模型。

### IE盒模型和W3C标准盒模型的区别是什么？

    1. W3C 标准盒模型：
> 属性width,height只包含内容content，不包含border和padding。

    2. IE 盒模型：
> 属性width,height包含border和padding，指的是content+padding+border。

> 在ie8+浏览器中使用哪个盒模型可以由box-sizing(CSS新增的属性)控制，默认值为content-box，即标准盒模型；如果将box-sizing设为border-box则用的是IE盒模型。如果在ie6,7,8中DOCTYPE缺失会触发IE模式。在当前W3C标准中盒模型是可以通过box-sizing自由的进行切换的。

> content-box（标准盒模型）

> width = 内容的宽度

> height = 内容的高度

> border-box（IE盒模型）

> width = border + padding + 内容的宽度

> height = border + padding + 内容的高度

