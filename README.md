select
======

A micro css selector engine

## 选择器支持

### 简单选择器

* #id
* .class
* tag
* tag.class
* tag#id
* *

### 子元素选择器

* tag > tag
* tag > .calss
* #id > #id
* ...

### 组选择器

* tag tag
* tag .class
* #id tag tag
* ...

## 注意

*  不支持 #id.class
*  尽可能使用子元素选择器(parent>child)而非组合选择器(parent child)
*  不支持含有通配符 * 的组合选择器
*  其他选择器可通过filter(elem,index,nodes)回调函数间接实现

## 参考

* http://ejohn.org/blog/selectors-that-people-actually-use/
* http://ejohn.org/blog/thoughts-on-queryselectorall/
* http://github.com/jeresig/sizzle
* http://james.padolsey.com/javascript/mini/