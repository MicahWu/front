# 文本样式

## text-indent 文本首行缩进
以px,pt,em,%设置的距离值

## text-align 文本水平对齐
* left
* center 居中对齐
* right
* justify 两端对齐
* inherit

## vertical-align 垂直对齐
* text-top 顶端对齐
* middle
* bottom
* ...

## white-space 空格处理
* normal
* nowrap 文本不自动换行 直到遇到<br/>
* pre 类似<pre>
* pre-line
* pre-wrap
* inherit

## ::first-letter 首字样式
```css
p::first-letter{
  font-size: 30px;
}
```
## ::first-line 首行样式
```css
p::first-line{
  font-size: 30px;
}
```
## 间距
* 行高 line-height (行高=行间距+文字高度)
* 字间距 letter-spacing

## text-decoration 文字装饰
* none
* underline 下划线
* overline 上划线
* line-through 中划线
* inherit

## text-shadow 文本阴影
* 水平 垂直 [,模糊距离,阴影颜色]
```css
h1{
  text-shadow: 16px 6px 15px red;
}
```
