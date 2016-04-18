# iframeMessage

## 简介

页面中有2个及以上个iframe时，iframe之间的数据传递通过该框架来实现。

## 使用方法

* 依赖jQuery
* 主页面引用mp.js
* 嵌套的iframe页面也引用mp.js
* 发送消息
    
```javascript
    MP.send('msg',{ sayHi:"hello world" });

```

* 接受消息

```javascript
 MP.on('msg',function(data){
     console.log(data['sayHi']) //hello world
})
```

* 效果

![mp_01](/example/mp_01.png)

