# flexbox
弹性盒模型笔记

## Flex布局

> 一维布局模型：一次只能处理一个维度（一行或者一列）上的元素布局

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [写给自己看的display: flex布局教程](https://www.zhangxinxu.com/wordpress/2018/10/display-flex-css3-css/#align-content)
- [30分钟彻底弄懂flex布局](https://www.cnblogs.com/qcloud1001/p/9848619.html)
- [flexboxfroggy，小游戏掌握flex布局的属性](https://flexboxfroggy.com/)



#### 作用在flex容器上的属性（控制整体）
属性名称 | 取值 | 默认值
---|---|---
flex-direction | `row | row-reverse | column | column-reverse` | row
flex-wrap | `nowrap | wrap | wrap-reverse` | nowrap
flex-flow  | `<flex-direction> || <flex-wrap>` | 
justify-content | `flex-start | flex-end | center | space-between | space-around | space-evenly` | flex-start
align-items | `stretch | flex-start | flex-end | center | baseline` | stretch
align-content | `flex-start | flex-end | center | space-between | space-around | stretch` | flex-start



#### 作用在flex子项上的属性（控制个体）
属性名称 | 取值 | 默认值
---|---|---
order | `<integer>` | 0
flex-grow | `<number>` | 0
flex-shrink | `<number>` | 1
flex-basis | `<length> | auto` | auto
flex | `<flex-grow> || <flex-shrink> || <flex-basis> ` | 0 1 auto
align-self | `auto | flex-start | flex-end | center | baseline | stretch` | auto继承父元素`align-items`

flex属性一些简写
> `flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ];`
```
flex: 1 = flex: 1 1 0%
flex: 2 = flex: 2 1 0%
flex: auto = flex: 1 1 auto;
flex: none = flex: 0 0 auto; // 常用于固定尺寸 不伸缩
```


#### 浏览器支持程度
- [flex支持程度](https://caniuse.com/#search=flex) (IE10+)

#### 总结