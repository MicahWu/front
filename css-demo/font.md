# font 字体
* font-style
* font-variant
* font-weight
* font-size
* font-family

## font-family 字体
### CSS通用字体
* Monospace 等宽字体
* Cursive 手写体
* Serif 不等宽，笔画末端有短线
* Sans-serif 不等宽，笔画末端无断线
* Fantasy 其他

## font-style 字体风格
* normal
* italic 斜体
* oblique 文本斜体
* inherit

## font-variant 字体变形
* normal
* small-caps
* inherit

## font-weight 字体粗细
* 名称方式
  * normal
  * bold 粗体
  * bolder 更粗
  * lighter 更细
  * inherit
* 数值方式
  * 100~900 值越小越细 400=normal 700=bold

## font-size 字体大小
* px 像素（屏幕上的一个点） 默认16px
* em 1em相当于当前字体大小
* % 基于父元素计算百分比
---
# 自定义字体
```css
@font-face{
  font-family: 自定义字体名;
  src:url(字体url地址);
}
```
