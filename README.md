# chimee-helper-dom

[![Build Status](https://img.shields.io/travis/Chimeejs/chimee-helper-dom/master.svg?style=flat-square)](https://travis-ci.org/Chimeejs/chimee-helper-dom.svg?branch=master)
[![Coverage Status](https://img.shields.io/coveralls/Chimeejs/chimee-helper-dom/master.svg?style=flat-square)](https://coveralls.io/github/Chimeejs/chimee-helper-dom?branch=master)
[![npm](https://img.shields.io/npm/v/chimee-helper-dom.svg?colorB=brightgreen&style=flat-square)](https://www.npmjs.com/package/chimee-helper-dom)
[![dependency Status](https://david-dm.org/Chimeejs/chimee-helper-dom.svg)](https://david-dm.org/Chimeejs/chimee-helper-dom)
[![devDependency Status](https://david-dm.org/Chimeejs/chimee-helper-dom/dev-status.svg)](https://david-dm.org/Chimeejs/chimee-helper-dom?type=dev)

dom handler of chimee

## get started

```shell
npm install chimee-helper-dom --save
```

if you are using `flow`, you should import our flow defination, by adding this to your `.flowconfig`.

    [ignore]

    [include]

    [libs]
    ./node_modules/chimee-helper-dom/lib/index.flow.js
    [options]

    [lints]

## doc

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### dom

[src/index.js:11-11](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L11-L11 "Source code on GitHub")

一些常用的DOM判断及操作方法，可以使用dom.$('\*')包装DOM，实现类jQuery的链式操作；当然这里的静态方法也可以直接使用。

**Meta**

-   **author**: huzunjie

### getAttr

[src/index.js:22-24](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L22-L24 "Source code on GitHub")

读取HTML元素属性值

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `attrName` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 目标属性名称

Returns **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 

### setAttr

[src/index.js:32-38](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L32-L38 "Source code on GitHub")

设置HTML元素属性值

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `attrName` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 目标属性名称
-   `attrVal` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 目标属性值

### addClassName

[src/index.js:45-59](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L45-L59 "Source code on GitHub")

为HTML元素添加className

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `cls` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要添加的className（多个以空格分割）

### removeClassName

[src/index.js:66-84](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L66-L84 "Source code on GitHub")

为HTML元素移除className

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `cls` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要移除的className（多个以空格分割）

### hasClassName

[src/index.js:92-94](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L92-L94 "Source code on GitHub")

检查HTML元素是否已设置className

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `className` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要检查的className

Returns **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 

### supportsPassive

[src/index.js:100-100](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L100-L100 "Source code on GitHub")

addEventListener 是否已支持 passive

Returns **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 

### removeEvent

[src/index.js:118-130](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L118-L130 "Source code on GitHub")

为HTML元素移除事件监听

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `once` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否只监听一次 (optional, default `false`)
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段的监听 (optional, default `false`)

### addEvent

[src/index.js:140-157](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L140-L157 "Source code on GitHub")

为HTML元素添加事件监听

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `once` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否只监听一次 (optional, default `false`)
-   `capture` **([Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean) \| [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object))** 是否在捕获阶段监听，这里也可以传入 { passive: true } 表示被动模式 (optional, default `false`)

### addDelegate

[src/index.js:167-191](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L167-L191 "Source code on GitHub")

为HTML元素添加事件代理

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要被代理的元素
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

### removeDelegate

[src/index.js:201-208](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L201-L208 "Source code on GitHub")

为HTML元素移除事件代理

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要被代理的元素
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

### getStyle

[src/index.js:216-218](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L216-L218 "Source code on GitHub")

读取HTML元素样式值

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `key` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 样式key

Returns **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 

### setStyle

[src/index.js:226-234](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L226-L234 "Source code on GitHub")

设置HTML元素样式值

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `key` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 样式key
-   `val` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 样式值

### query

[src/index.js:243-246](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L243-L246 "Source code on GitHub")

根据选择器查询目标元素

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 选择器,用于 querySelectorAll
-   `container` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 父容器 (optional, default `document`)
-   `toArray` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 强制输出为数组

Returns **([NodeList](https://developer.mozilla.org/en-US/docs/Web/API/NodeList) \| [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array))** 

### removeEl

[src/index.js:252-254](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L252-L254 "Source code on GitHub")

从DOM树中移除el

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素

### findParents

[src/index.js:263-276](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L263-L276 "Source code on GitHub")

查找元素的父节点们

**Parameters**

-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 目标元素
-   `endEl` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 最大父容器（不指定则找到html） (optional, default `null`)
-   `haveEl` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 包含当前元素
-   `haveEndEl` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 包含设定的最大父容器

### $

[src/index.js:284-286](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L284-L286 "Source code on GitHub")

根据选择器查询并得到目标元素的wrap包装器

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 选择器,另外支持 HTMLString||NodeList||NodeArray||HTMLElement
-   `container` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 父容器

Returns **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** 

### NodeWrap

[src/index.js:297-552](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L297-L552 "Source code on GitHub")

NodeWrap DOM包装器，用以实现基本的链式操作
new dom.NodeWrap('_') 相当于 dom.$('_')
这里面用于DOM操作的属性方法都是基于上面静态方法实现，有需要可以随时修改补充

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 选择器(兼容 String||HTMLString||NodeList||NodeArray||HTMLElement)
-   `container` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 父容器（默认为document） (optional, default `document`)

#### each

[src/index.js:335-338](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L335-L338 "Source code on GitHub")

循环遍历DOM集合

**Parameters**

-   `args` **...any** 
-   `fn` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 遍历函数 fn(item, i)

Returns **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** 

#### push

[src/index.js:345-348](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L345-L348 "Source code on GitHub")

添加元素到DOM集合

**Parameters**

-   `args` **...any** 
-   `el` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 要加入的元素

Returns **this** 

#### splice

[src/index.js:356-358](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L356-L358 "Source code on GitHub")

截取DOM集合片段，并得到新的包装器splice

**Parameters**

-   `args` **...any** 
-   `start` **Nubmer** 
-   `count` **Nubmer** 

Returns **[NodeWrap](#nodewrap)** 新的DOM集合包装器

#### find

[src/index.js:365-374](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L365-L374 "Source code on GitHub")

查找子元素

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 选择器

Returns **[NodeWrap](#nodewrap)** 新的DOM集合包装器

#### append

[src/index.js:381-386](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L381-L386 "Source code on GitHub")

添加子元素

**Parameters**

-   `childEls` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 要添加的HTML元素

Returns **this** 

#### appendTo

[src/index.js:393-396](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L393-L396 "Source code on GitHub")

将元素集合添加到指定容器

**Parameters**

-   `parentEl` **[HTMLElement](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)** 要添加到父容器

Returns **this** 

#### text

[src/index.js:403-410](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L403-L410 "Source code on GitHub")

DOM集合text内容读写操作

**Parameters**

-   `val` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 文本内容（如果有设置该参数则执行写操作，否则执行读操作）

Returns **this** 

#### html

[src/index.js:417-424](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L417-L424 "Source code on GitHub")

DOM集合HTML内容读写操作

**Parameters**

-   `html` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** html内容（如果有设置该参数则执行写操作，否则执行读操作）

Returns **this** 

#### attr

[src/index.js:432-437](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L432-L437 "Source code on GitHub")

DOM集合属性读写操作

**Parameters**

-   `name` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 属性名称
-   `val` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 属性值（如果有设置该参数则执行写操作，否则执行读操作）

Returns **this** 

#### data

[src/index.js:445-455](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L445-L455 "Source code on GitHub")

DOM集合dataset读写操作

**Parameters**

-   `key` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 键名
-   `val` **Any** 键值（如果有设置该参数则执行写操作，否则执行读操作）

Returns **this** 

#### css

[src/index.js:463-468](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L463-L468 "Source code on GitHub")

DOM集合样式读写操作

**Parameters**

-   `key` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 样式key
-   `val` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 样式值（如果有设置该参数则执行写操作，否则执行读操作）

Returns **this** 

#### addClass

[src/index.js:475-477](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L475-L477 "Source code on GitHub")

为DOM集合增加className

**Parameters**

-   `cls` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要增加的className

Returns **this** 

#### removeClass

[src/index.js:484-486](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L484-L486 "Source code on GitHub")

移除当前DOM集合的className

**Parameters**

-   `cls` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要移除的className

Returns **this** 

#### hasClass

[src/index.js:493-495](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L493-L495 "Source code on GitHub")

检查索引0的DOM是否有className

**Parameters**

-   `cls` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 要检查的className

Returns **this** 

#### on

[src/index.js:505-507](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L505-L507 "Source code on GitHub")

为DOM集合添加事件监听

**Parameters**

-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `once` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否只监听一次 (optional, default `false`)
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

Returns **this** 

#### off

[src/index.js:517-519](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L517-L519 "Source code on GitHub")

为DOM集合解除事件监听

**Parameters**

-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `once` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否只监听一次 (optional, default `false`)
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

Returns **this** 

#### delegate

[src/index.js:529-531](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L529-L531 "Source code on GitHub")

为DOM集合绑定事件代理

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 目标子元素选择器
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

Returns **this** 

#### undelegate

[src/index.js:541-543](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L541-L543 "Source code on GitHub")

为DOM集合解绑事件代理

**Parameters**

-   `selector` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 目标子元素选择器
-   `type` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 事件名称
-   `handler` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 处理函数
-   `capture` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** 是否在捕获阶段监听 (optional, default `false`)

Returns **this** 

#### remove

[src/index.js:549-551](https://github.com/Chimeejs/chimee-helper-dom/blob/f4846df3756281209bdf89873827bfcbd5451ba4/src/index.js#L549-L551 "Source code on GitHub")

从DOM树中移除

Returns **this** 
