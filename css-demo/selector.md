# css选择器

## 类型/元素选择器
```css
p{
  color: red
}
```
## 后代选择器
所有后代
```css
p em{
  color: red
}
```
## ID选择器
```css
#test{
  color: red
}
```
## 类选择器
```css
.test{
  color: red
}
```
## 群组选择器
```css
p, #test, .test {
  color: red
}
```
## 伪类选择器
第一个P标签
```css
p:first-child {
  color: red
}
```
## 通用选择器
```css
*{
  color: red
}
```
## 子选择器
直接后代
```css
#cc > li {
  color: red
}
```
## 属性选择器
```css
p[id^='tt'] {
  color: red
}
```
## 兄弟选择器
```css
h1+p {
  color: red
}
```
