# cssreset
css style reset by linfs

2017-08-31 created

> 有margin值的元素有：

`body` `h1` `h2` `h3` `h4` `h5` `h6` `p` `blockquote` `pre` `hr` `figure` `dl` `dd` `ul` `ol` `fieldset` `menu`

> 有padding值的元素有:

`ul` `ol` `button` `th` `td` `fieldset` `legend` `textarea` `menu`

> 有border值的元素有：

`hr` `input` `button` `fieldset` `textarea`

虽然这些都有border,不过个人觉得没有必要进行重置。

```css
body,h1,h2,h3,h4,h5,h6,p,blockquote,pre,hr,figure, dl,dd,ul,ol,fieldset,menu{margin:0}
ul,ol,button,th,td,fieldset,legend,textarea,menu{padding:0}
```

##### HTML5新标签针对旧浏览器重置

```css
header,footer,section,article,aside,nav,hgroup,address,figure,figcaption,menu,details{display:block;}
```

##### 其它元素样式重置

###### body

```css
body{
line-height:1;
}
```

###### 字体大小

```css
h1,h2,h3,h4,h5,h6,pre{
font-size:100%;
}
```

###### 列表

```css
ol,ul{
list-style:none;
}
```

###### 表格

```css
table {
border-collapse: collapse;
border-spacing: 0;
}
```

###### 链接

```css
:link,:visited{
text-decoration:none;
}
```

###### 金手指

```css
a,button,input[type='button']{
cursor:pointer;
}
```

##### 利用伪类清除浮动

```css
.clearfix:after {
content:".";
display:block;
height:0;
visibility:hidden;
clear:both;
}
.clearfix {
*zoom:1;
}
```


查看 [cssreset](https://github.com/linfushan/FE/blob/master/cssreset.md)文件说明

更多css规范 [NEC](http://nec.netease.com/)

