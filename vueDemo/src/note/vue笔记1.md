### vue.js 笔记1
####MVVM结构

是前端开发的理念

主要把每个页面分成分为model，view，viewmodel

其中viewmodel是MVVM的核心，model是保存的数据，view是页面中的html代码

viewmodel作为调度机制，当view需要保存数时，
都需要viewmodel来进行处理

因为viewmodel提供了数据的双向绑定，所以这个思想方便了开发

#### Vue基本代码结构

1. 插值表达式

   + 写法为{{}}，用于将vue实例中的数据放入对应的DOM对象中
2. v-text
   + 写在标签属性中，会用变量的内容完全替换标签内的本来内容
3. v-cloak
   + 防止{{}}插入的内容因为加载缓慢而显示在页面上（防止闪烁）
4. v-html
   + 将实例变量内容作为HTML标签
5. v-bind
   + 属性绑定机制，避免取不到Vue实例中的值，缩写是：
6. v-on
   + 事件绑定机制，将Vue实例中的methods中定义的函数，绑定到事件上，缩写是@
   + 另外，在v-on中可以使用stop，prevent，capture，self，once修饰符来进行触发事件的调用调整
7. v-model
   + Vue中唯一一个可以对 View 和 Model 进行双向数据绑定的组件，v-bind只能把Model绑定到View上去，只有
   使用v-model才能将View的改动实时反映到Model上
8. v-for
   + v-for可以用来循环，可以循环数组，对象数组，对象和纯数字
9. v-if
   + v-if用于条件判断，但是v-if会将判定为false的DOM对象直接删除
10. v-show
   + v-show也可以条件判断，但是会将判定为false的DOM对象设置为不可见，并不直接删除对象

   
