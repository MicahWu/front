# 颜色与背景样式

## 颜色表示
* 颜色名 red green blue
* rgb(x,x,x)
* rgb(x%, x%, x%)
* #rrggbb

## 渐变
* linear-gradient(渐变方向, 颜色停靠点1, 颜色停靠点2,...)
* radial-gradient(形状, 颜色停靠点1, 颜色停靠点2,...)
前缀兼容
-webkit-
-o-
-moz-

---
# background
* background-color
* background-image
* background-repeat
* background-attachment
* background-position

## color 文本颜色
## background-color 背景颜色
## background-image 背景图片
```csss
 div{
   background-image:url('path/to/img');
 }
```
## background-repeat 背景图片平铺方式
* repeat
* repeat-x
* repeat-y
* no-repeat
## background-attachment 固定背景图片
* scroll 默认
* fixed 不会随页面滚动而滚动
## background-position 背景图片定位 配合no-repeat
* 数值
* left
* right
* center
