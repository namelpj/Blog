---
title: React表单组件
date: 2017-04-17 14:22:09
tags:
---
1、像是input、textarea、option这样的表单组件不同于其他组件，因为他们可以通过用户交互发生变化。这些组件提供的界面使响应用户交互的表单数据处理更加容易。
2、交互属性
表单组件支持几个受用户交互影响的属性
value，用于input、textarea组件；checked，用于类型为checkbox或者radio的input组件；selected，用于option组件。
在HTML中，textarea的值通过子节点设置，在React中则应该使用value代替。表单组件可以通过onChange会调函数来监听组件变化。当用户做出以下交互时，onChange执行并通过浏览器做出响应：

* input 或 textarea 的 value 发生变化时。
* input 的 checked 状态改变时。
* option 的 selected 状态改变时。

和所有的DOM事件一样，所有的HTML原生组件都支持onChange属性，而且可以用来监听冒泡的change事件。