

# CSS优先级

## 内联 > 内部 > 外部

1. `<div style="..."/>`

2. `<style type='media'>...</style>`

3. `<link rel='stylesheet' href='path/to/css/file'/>`


## important > 内嵌样式 > ID > 类 > 标签 | 伪类 | 属性选择 > 伪对象 > 继承 > 通配符
```
important的权重为1,0,0,0
ID的权重为0,1,0,0
类的权重为0,0,1,0
标签的权重为0,0,0,1
伪类的权重为0,0,1,0
属性的权重为0,0,1,0
伪对象的权重为0,0,0,1
通配符的权重为0,0,0,0
```

```
   *             {}  /* a=0 b=0 c=0 d=0 -> specificity = 0,0,0,0 */
   li            {}  /* a=0 b=0 c=0 d=1 -> specificity = 0,0,0,1 */
   li:first-line {}  /* a=0 b=0 c=0 d=2 -> specificity = 0,0,0,2 */
   ul li         {}  /* a=0 b=0 c=0 d=2 -> specificity = 0,0,0,2 */
   ul ol+li      {}  /* a=0 b=0 c=0 d=3 -> specificity = 0,0,0,3 */
   h1 + *[rel=up]{}  /* a=0 b=0 c=1 d=1 -> specificity = 0,0,1,1 */
   ul ol li.red  {}  /* a=0 b=0 c=1 d=3 -> specificity = 0,0,1,3 */
   li.red.level  {}  /* a=0 b=0 c=2 d=1 -> specificity = 0,0,2,1 */
   #x34y         {}  /* a=0 b=1 c=0 d=0 -> specificity = 0,1,0,0 */
   style=""          /* a=1 b=0 c=0 d=0 -> specificity = 1,0,0,0 */
   ```
