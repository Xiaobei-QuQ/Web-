# 小北音乐电台

## 项目功能介绍

主要模块是实现了音乐电台的在线播放和各种电台的切换。包括下一曲，播放暂停，进度条显示时间，歌词滚动显示，滑动显示分类电台，专辑和背景图的切换等功能。

## 项目技术细节介绍

项目主要技术为ES5,ES6,jQuery，通过ajax取数据渲染页面，通过事件中心管理机制实现事件绑定，通过animate.css实现歌词动态显示，通过获取audio信息获取进度条长度，播放信息。

遇到的问题是事件中心管理机制难以理解
```
var EventCenter = {
    on: function (type,handler) {
        $(document).on(type,handler)
    },
    fire: function (type,data) {
        $(document).trigger(type,data)
    }
}
// EventCenter.on('hello',function (e) {
//     console.log(e.detail)
// })
// EventCenter.fire('hello','你好')
```
通过这个中心实现各模块互相独立，互不影响。解决的方法是了解了自定义事件以及面向对象的代码写法。

## 项目收货

这个项目耗时不久，做得比较一般，日后可以找时间实现以下功能

- 进度条快进
- 音量调节
- 收藏
- 点赞

## 技术栈

jQuery CSS3 响应式 ES5 ES6 
