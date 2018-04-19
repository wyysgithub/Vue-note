# Vue 学习笔记

[官方文档](https://cn.vuejs.org)

首次尝试：

文件：[index.html](https://github.com/wyysgithub/Vue-note/blob/master/index.html)

![](https://github.com/wyysgithub/Vue-note/blob/master/img/helloVue.png)


## 知识点总结：

#### 1，使用el通过元素id挂载DOM。

#### 2，使用data创建数据。

#### 3，引入数据的方式：

* 使用插值表达式{{msg}}引入数据

* 使用v-text和v-html引入数据

`v-text 会转译 v-html 不会`

#### 4，使用methods定义函数。

**函数中可以用this.msg修改data中的数据，Vue会自主更新**

#### 5，绑定事件

* 使用v-on绑定

* 使用@绑定



# 2-4 属性绑定和双向数据绑定

文件：[index2-4.html](https://github.com/wyysgithub/Vue-note/blob/master/index2-4.html)

![](https://github.com/wyysgithub/Vue-note/blob/master/img/index2-4.png)

## 2-4 知识点总结：

#### 1，使用v-bind绑定属性

`"v-bind："可直接缩写成":"`

#### 2，使用v-model双向绑定。


# 2-5 计算属性与侦听器

文件：[index2-5.html](https://github.com/wyysgithub/Vue-note/blob/master/index2-5.html)

![](https://github.com/wyysgithub/Vue-note/blob/master/img/index2-5.png)

## 2-5 知识点总结：

#### 1，使用computed定义计算属性


#### 2，使用watch创建监听。


# 2-6 v-if,v-show,v-for指令

文件：[index2-6.html](https://github.com/wyysgithub/Vue-note/blob/master/index2-6.html)

![](https://github.com/wyysgithub/Vue-note/blob/master/img/index2-6.png)

## 2-6 知识点总结：

#### 1，隐藏元素

* 使用v-if移除或添加元素。


* 使用v-show显示或者隐藏元素。

两者均为布尔类型，差别在于v-if是直接移除，v-show是修改display属性。

#### 2，v-for 循环遍历

> <li v-for="(item,index) of list" :key="index">{{item}}</li>

* v-for 需设置遍历所用的key，key值也可直接使用item，但在数组内有相同元素的时候不适用，所以用index数组角标做key。

使用 v-for="item in list"  或者 v-for="item of list" 进行遍历

使用list:list:[{n:1},{n:2},{n:3},{n:4},{n:5},{n:6}] 时为了方便扩展， 更贴近实际项目需求。









